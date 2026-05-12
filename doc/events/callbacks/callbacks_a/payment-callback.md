
# Payment Callback

Called when payment processing is complete

## Signature Verification

This event uses the `HMAC Signature Verifier` for request verification. The event includes an `X-Signature` header that will be validated using your shared `secret-key` to ensure request authenticity.

## Headers

This event's request contains the following headers.

| Name |
|  --- |
| Content-Type |

## Payload Type

This event's request payload is of type [PaymentCallback](../../../../doc/models/payment-callback.md).

## Payload Example

```json
{
  "orderId": "order_789",
  "paymentStatus": "success",
  "transactionId": "txn_abc123",
  "amount": 59.98,
  "currency": "USD",
  "timestamp": "2025-09-19T10:35:00Z",
  "failureReason": "failureReason2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

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

## Accepted Server Responses

The server should responds with one of the following status codes:

| Status Code | Description |
|  --- | --- |
| 200 | Callback received successfully |
| 400 | Invalid callback data |

