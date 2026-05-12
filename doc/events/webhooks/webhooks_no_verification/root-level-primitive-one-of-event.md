
# Root Level Primitive One of Event

Root-level oneOf across primitives and collections of primitives/enums.

## Headers

This event's request contains the following headers.

| Name |
|  --- |
| Content-Type |

## Payload Type

This event's request payload is of type [RootLevelOneOfPrimitiveEventRootLevelPrimitiveOneOfBody](../../../../doc/models/containers/root-level-one-of-primitive-event-root-level-primitive-one-of-body.md).

## Payload Example

```json
"on"
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
import localhost3000.events.webhooks.WebhooksNoVerificationHandler;
import localhost3000.events.webhooks.WebhooksNoVerificationParsingResult;
import localhost3000.http.request.HttpRequest;
import localhost3000.models.containers.RootLevelOneOfPrimitiveEventRootLevelPrimitiveOneOfBody;

@RestController
public class WebhooksNoVerificationController {

    @PostMapping("/webhooksnoverification")
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

        String result = WebhooksNoVerificationHandler.parseEventAsync(httpRequest).thenApply(webhooksNoVerificationParsingResult ->
            webhooksNoVerificationParsingResult.matchSome(new WebhooksNoVerificationParsingResult.SomeCases<String>() {
                @Override
                public String rootLevelPrimitiveOneOfEvent(RootLevelOneOfPrimitiveEventRootLevelPrimitiveOneOfBody rootLevelPrimitiveOneOfEvent) {
                    return MessageFormat.format("RootLevelPrimitiveOneOfEvent event received {0}", rootLevelPrimitiveOneOfEvent);
                }

                @Override
                public String unknown() {
                    return "Unknown event received";
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
| 200 | Event processed successfully |
| 422 | Event processing failed |

