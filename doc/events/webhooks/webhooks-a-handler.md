## Webhooks A Handler

Advanced webhook group for payment status events

## Signature Verification

This handler uses the `HMAC Signature Verifier` for request verification. Each event in this group includes an `X-Signature` header that will be validated using your shared `secret-key` to ensure request authenticity.

## Events

Events available in this group. Subscribe to receive webhook notifications when these events occur.

| Name | Description |
|  --- | --- |
| [paymentStatusUpdated](../../../doc/events/webhooks/webhooks_a/payment-status-updated.md) | Triggered when a payment status is updated via POST method |
| [paymentStatusCreated](../../../doc/events/webhooks/webhooks_a/payment-status-created.md) | Triggered when a new payment status is created |

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
import localhost3000.events.webhooks.WebhooksAHandler;
import localhost3000.events.webhooks.WebhooksAParsingResult;
import localhost3000.http.request.HttpRequest;
import localhost3000.models.PaymentStatusUpdatedEvent;
import localhost3000.models.PaymentStatusCreatedEvent;
import localhost3000.events.SignatureVerificationResult;

@RestController
public class WebhooksAController {

    @PostMapping("/webhooksa")
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
        WebhooksAHandler handler = new WebhooksAHandler("hmac-secret-key");

        String result = handler.verifyAndParseEventAsync(httpRequest).thenApply(webhooksAParsingResult ->
            webhooksAParsingResult.matchSome(new WebhooksAParsingResult.SomeCases<String>() {
                @Override
                public String paymentStatusUpdated(PaymentStatusUpdatedEvent paymentStatusUpdated) {
                    return MessageFormat.format("PaymentStatusUpdated event received {0}", paymentStatusUpdated.toString());
                }

                @Override
                public String paymentStatusCreated(PaymentStatusCreatedEvent paymentStatusCreated) {
                    return MessageFormat.format("PaymentStatusCreated event received {0}", paymentStatusCreated.toString());
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

