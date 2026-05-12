## Webhooks C Handler

Primitive and collection variant webhook group.

## Signature Verification

This handler uses the `HMAC Signature Verifier` for request verification. Each event in this group includes an `X-Webhook-Signature` header that will be validated using your shared `secret-key` to ensure request authenticity.

## Events

Events available in this group. Subscribe to receive webhook notifications when these events occur.

| Name |
|  --- |
| [stringEvent](../../../doc/events/webhooks/webhooks_c/string-event.md) |
| [intEvent](../../../doc/events/webhooks/webhooks_c/int-event.md) |
| [numberListEvent](../../../doc/events/webhooks/webhooks_c/number-list-event.md) |
| [stringMapEvent](../../../doc/events/webhooks/webhooks_c/string-map-event.md) |

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
import localhost3000.events.webhooks.WebhooksCHandler;
import localhost3000.events.webhooks.WebhooksCParsingResult;
import localhost3000.http.request.HttpRequest;
import java.util.List;
import localhost3000.events.SignatureVerificationResult;

@RestController
public class WebhooksCController {

    @PostMapping("/webhooksc")
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
        WebhooksCHandler handler = new WebhooksCHandler("hmac-secret-key");

        String result = handler.verifyAndParseEventAsync(httpRequest).thenApply(webhooksCParsingResult ->
            webhooksCParsingResult.matchSome(new WebhooksCParsingResult.SomeCases<String>() {
                @Override
                public String stringEvent(String stringEvent) {
                    return MessageFormat.format("StringEvent event received {0}", stringEvent);
                }

                @Override
                public String intEvent(int intEvent) {
                    return MessageFormat.format("IntEvent event received {0}", intEvent);
                }

                @Override
                public String numberListEvent(List<Double> numberListEvent) {
                    return MessageFormat.format("NumberListEvent event received {0}", numberListEvent);
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

