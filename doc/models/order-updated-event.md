
# Order Updated Event

*This model accepts additional fields of type Object.*

## Structure

`OrderUpdatedEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `EventType` | [`EventType`](../../doc/models/event-type.md) | Optional | - | EventType getEventType() | setEventType(EventType eventType) |
| `OrderUpdatedId` | `int` | Required | - | int getOrderUpdatedId() | setOrderUpdatedId(int orderUpdatedId) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "orderUpdatedId": 91,
  "eventType": "order.updated",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

