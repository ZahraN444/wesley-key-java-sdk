## Webhooks B Handler

Multi-event webhook group with oneOf payload structures. Uses a message template that also includes a request header pointer.

## Signature Verification

This handler uses the `HMAC Signature Verifier` for request verification. Each event in this group includes an `X-Webhook-Signature` header that will be validated using your shared `secret-key` to ensure request authenticity.

## Events

Events available in this group. Subscribe to receive webhook notifications when these events occur.

| Name | Description |
|  --- | --- |
| [userNotificationEvent](../../../doc/events/webhooks/webhooks_b/user-notification-event.md) | Triggered when user-related notifications occur |
| [systemNotificationEvent](../../../doc/events/webhooks/webhooks_b/system-notification-event.md) | Triggered when system-wide notifications occur |
| [inventoryChangeEvent](../../../doc/events/webhooks/webhooks_b/inventory-change-event.md) | Triggered when inventory stock levels change |

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
import localhost3000.events.webhooks.WebhooksBHandler;
import localhost3000.events.webhooks.WebhooksBParsingResult;
import localhost3000.http.request.HttpRequest;
import localhost3000.models.containers.UserNotificationEventBody;
import localhost3000.models.containers.SystemNotificationEventBody;
import localhost3000.models.containers.InventoryChangeEventBody;
import localhost3000.events.SignatureVerificationResult;

@RestController
public class WebhooksBController {

    @PostMapping("/webhooksb")
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
        WebhooksBHandler handler = new WebhooksBHandler("hmac-secret-key");

        String result = handler.verifyAndParseEventAsync(httpRequest).thenApply(webhooksBParsingResult ->
            webhooksBParsingResult.matchSome(new WebhooksBParsingResult.SomeCases<String>() {
                @Override
                public String userNotificationEvent(UserNotificationEventBody userNotificationEvent) {
                    return MessageFormat.format("UserNotificationEvent event received {0}", userNotificationEvent);
                }

                @Override
                public String systemNotificationEvent(SystemNotificationEventBody systemNotificationEvent) {
                    return MessageFormat.format("SystemNotificationEvent event received {0}", systemNotificationEvent);
                }

                @Override
                public String inventoryChangeEvent(InventoryChangeEventBody inventoryChangeEvent) {
                    return MessageFormat.format("InventoryChangeEvent event received {0}", inventoryChangeEvent);
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

