
# Payment Status Created Event

*This model accepts additional fields of type Object.*

## Structure

`PaymentStatusCreatedEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PaymentStatusCreatedId` | `String` | Required | - | String getPaymentStatusCreatedId() | setPaymentStatusCreatedId(String paymentStatusCreatedId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "paymentStatusCreatedId": "ps_123",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

