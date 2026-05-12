
# Fulfillment Callback

Called when order processing is complete

## Signature Verification

This event uses the `HMAC Signature Verifier` for request verification. The event includes an `X-Signature` header that will be validated using your shared `secret-key` to ensure request authenticity.

## Headers

This event's request contains the following headers.

| Name |
|  --- |
| Content-Type |

## Payload Type

This event's request payload is of type [FulfillmentCallback](../../../../doc/models/fulfillment-callback.md).

## Payload Example

```json
{
  "orderId": null,
  "fulfillmentStatus": "fulfilled",
  "carrier": "FedEx",
  "estimatedDelivery": "2025-09-22",
  "timestamp": "2025-09-19T14:00:00Z",
  "totalWeight": 12.75,
  "price": 199.99,
  "quantity": 5,
  "longId": 9223372036854775807,
  "fragile": true,
  "items": [
    "item1",
    "item2"
  ],
  "packages": [
    {
      "packageId": "PKG123",
      "weight": 2.5
    }
  ],
  "address": {
    "street": "123 Main St",
    "city": "New York",
    "zip": "10001"
  },
  "metadata": {
    "customField1": "value",
    "customField2": 123
  },
  "attributes": {
    "color": "red",
    "size": "XL"
  },
  "deliveryDetails": {
    "method": "express",
    "eta": "2025-09-21T12:00:00Z"
  },
  "fulfillmentStatuss": "fulfilled",
  "carrierr": "FedEx",
  "estimatedDeliveryy": "2025-09-22",
  "timestampp": "2025-09-19T14:00:00Z",
  "trackingNumber": "trackingNumber4",
  "scopes": [
    "test1",
    "selection",
    "file_requests.read"
  ],
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

## Accepted Server Responses

The server should responds with one of the following status codes:

| Status Code | Description |
|  --- | --- |
| 200 | Callback acknowledged |
| 422 | Callback processing failed |

