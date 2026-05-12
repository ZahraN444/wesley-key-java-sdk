## Callbacks B Handler

Notification delivery callback group with discriminator mapping

Events in this group are uniquely identified by the `notificationType` field.

## Signature Verification

This handler uses the `HMAC Signature Verifier` for request verification. Each event in this group includes an `X-Signature` header that will be validated using your shared `secret-key` to ensure request authenticity.

## Events

Events available in this group. Subscribe to receive webhook notifications when these events occur.

| Name | Description | Event Identifier |
|  --- | --- | --- |
| [emailNotificationCallback](../../../doc/events/callbacks/callbacks_b/email-notification-callback.md) | Called when email notification delivery is complete | email |
| [smsNotificationCallback](../../../doc/events/callbacks/callbacks_b/sms-notification-callback.md) | Called when SMS notification delivery is complete | sms |

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
import localhost3000.events.callbacks.CallbacksBHandler;
import localhost3000.events.callbacks.CallbacksBParsingResult;
import localhost3000.http.request.HttpRequest;
import localhost3000.models.NotificationCallback;
import localhost3000.events.SignatureVerificationResult;

@RestController
public class CallbacksBController {

    @PostMapping("/callbacksb")
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
        CallbacksBHandler handler = new CallbacksBHandler("hmac-secret-key");

        String result = handler.verifyAndParseEventAsync(httpRequest).thenApply(callbacksBParsingResult ->
            callbacksBParsingResult.matchSome(new CallbacksBParsingResult.SomeCases<String>() {
                @Override
                public String emailNotificationCallback(NotificationCallback emailNotificationCallback) {
                    return MessageFormat.format("EmailNotificationCallback event received {0}", emailNotificationCallback.toString());
                }

                @Override
                public String smsNotificationCallback(NotificationCallback smsNotificationCallback) {
                    return MessageFormat.format("SmsNotificationCallback event received {0}", smsNotificationCallback.toString());
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

