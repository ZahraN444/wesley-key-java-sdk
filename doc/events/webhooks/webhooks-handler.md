## Webhooks Handler

Standard webhook group for order and payment events

## Signature Verification

This handler uses the `HMAC Signature Verifier` for request verification. Each event in this group includes an `X-Signature` header that will be validated using your shared `secret-key` to ensure request authenticity.

## Events

Events available in this group. Subscribe to receive webhook notifications when these events occur.

| Name | Description |
|  --- | --- |
| [orderCreated new testing my newy tesingggggg toc hejcjk](../../../doc/events/webhooks/webhooks/order-created-new-testing-my-newy-tesingggggg-toc-hejcjk.md) | Triggered when a new order is created |
| [orderUpdated](../../../doc/events/webhooks/webhooks/order-updated.md) | Triggered when an order is updated |
| [paymentCompleted](../../../doc/events/webhooks/webhooks/payment-completed.md) | Triggered when a payment is successfully processed |
| [primitiveCollectionEvent](../../../doc/events/webhooks/webhooks/primitive-collection-event.md) | Demonstrates oneOf across enum(string), integer, and array types. |

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
import localhost3000.events.webhooks.WebhooksHandler;
import localhost3000.events.webhooks.WebhooksParsingResult;
import localhost3000.http.request.HttpRequest;
import localhost3000.models.OrderCreatedEvent;
import localhost3000.models.OrderUpdatedEvent;
import localhost3000.models.PaymentCompletedEvent;
import localhost3000.events.SignatureVerificationResult;

@RestController
public class WebhooksController {

    @PostMapping("/webhooks")
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
        WebhooksHandler handler = new WebhooksHandler("hmac-secret-key");

        String result = handler.verifyAndParseEventAsync(httpRequest).thenApply(webhooksParsingResult ->
            webhooksParsingResult.matchSome(new WebhooksParsingResult.SomeCases<String>() {
                @Override
                public String orderCreatedNewTestingMyNewyTesinggggggTocHejcjk(OrderCreatedEvent orderCreatedNewTestingMyNewyTesinggggggTocHejcjk) {
                    return MessageFormat.format("OrderCreatedNewTestingMyNewyTesinggggggTocHejcjk event received {0}", orderCreatedNewTestingMyNewyTesinggggggTocHejcjk.toString());
                }

                @Override
                public String orderUpdated(OrderUpdatedEvent orderUpdated) {
                    return MessageFormat.format("OrderUpdated event received {0}", orderUpdated.toString());
                }

                @Override
                public String paymentCompleted(PaymentCompletedEvent paymentCompleted) {
                    return MessageFormat.format("PaymentCompleted event received {0}", paymentCompleted.toString());
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

