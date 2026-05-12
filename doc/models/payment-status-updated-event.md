
# Payment Status Updated Event

*This model accepts additional fields of type Object.*

## Structure

`PaymentStatusUpdatedEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PaymentStatusId` | `String` | Required | - | String getPaymentStatusId() | setPaymentStatusId(String paymentStatusId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "paymentStatusId": "ps_123",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

