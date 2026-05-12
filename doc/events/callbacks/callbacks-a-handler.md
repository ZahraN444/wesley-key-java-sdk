## Callbacks A Handler

Payment and fulfillment callback group with custom verification

## Signature Verification

This handler uses the `HMAC Signature Verifier` for request verification. Each event in this group includes an `X-Signature` header that will be validated using your shared `secret-key` to ensure request authenticity.

## Events

Events available in this group. Subscribe to receive webhook notifications when these events occur.

| Name | Description |
|  --- | --- |
| [paymentCallback](../../../doc/events/callbacks/callbacks_a/payment-callback.md) | Called when payment processing is complete |
| [fulfillmentCallback](../../../doc/events/callbacks/callbacks_a/fulfillment-callback.md) | Called when order processing is complete |

## SDK Usage Example

```java
package com.example.eventslistener;

import org.springframework.http.ResponseEntity;
import org.springframework.web.bind.annotation.PostMapping;
import org.springframework.web.bind.annotation.RequestBody;
import org.springframework.web.bind.annotation.RestController;
import javax.servlet.http.HttpServletRequest;
import java.text.MessageFormat;
import java.util.Collections;
import java.util.stream.Collectors;
import localhost3000.events.callbacks.CallbacksAHandler;
import localhost3000.events.callbacks.CallbacksAParsingResult;
import localhost3000.http.request.HttpRequest;
import localhost3000.models.PaymentCallback;
import localhost3000.models.FulfillmentCallback;
import localhost3000.events.SignatureVerificationResult;

@RestController
public class CallbacksAController {

    @PostMapping("/callbacksa")
    public ResponseEntity<String> receiveEvent(
            HttpServletRequest request,
            @RequestBody(required = false) String body) {

        // Create the HttpRequest from the incoming Request
        HttpRequest httpRequest = HttpRequest.fromHttpServletRequest(
                Collections.list(request.getHeaderNames()).stream().collect(Collectors.toMap(
                        h -> h,
                        h -> Collections.list(request.getHeaders(h))
                )),
                request.getParameterMap(),
                request.getRequestURL(),
                request.getQueryString(),
                request.getMethod(),
                body
        );

        // Use the provided handler to verify and parse the incoming event
        CallbacksAHandler handler = new CallbacksAHandler("hmac-secret-key");

        String result = handler.verifyAndParseEventAsync(httpRequest).thenApply(callbacksAParsingResult ->
            callbacksAParsingResult.matchSome(new CallbacksAParsingResult.SomeCases<String>() {
                @Override
                public String paymentCallback(PaymentCallback paymentCallback) {
                    return MessageFormat.format("PaymentCallback event received {0}", paymentCallback.toString());
                }

                @Override
                public String fulfillmentCallback(FulfillmentCallback fulfillmentCallback) {
                    return MessageFormat.format("FulfillmentCallback event received {0}", fulfillmentCallback.toString());
                }

                @Override
                public String unknown() {
                    return "Unknown event received";
                }

                @Override
                public String signatureVerificationFailed(SignatureVerificationResult signatureVerificationResult) {
                    return MessageFormat.format("SignatureVerificationResult event received {0}", signatureVerificationResult.toString());
                }

            })
        ).join();

        return ResponseEntity.status(200).body(result);
    }
}
```

