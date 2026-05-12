
# Payment Completed Event

*This model accepts additional fields of type Object.*

## Structure

`PaymentCompletedEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `EventType` | [`EventType1`](../../doc/models/event-type-1.md) | Optional | - | EventType1 getEventType() | setEventType(EventType1 eventType) |
| `PaymentId` | `int` | Required | - | int getPaymentId() | setPaymentId(int paymentId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "paymentId": 91,
  "eventType": "payment.completed",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

