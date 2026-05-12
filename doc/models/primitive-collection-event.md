
# Primitive Collection Event

*This model accepts additional fields of type Object.*

## Structure

`PrimitiveCollectionEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `EventType` | [`EventType2`](../../doc/models/event-type-2.md) | Optional | - | EventType2 getEventType() | setEventType(EventType2 eventType) |
| `Ids` | `List<Integer>` | Required | - | List<Integer> getIds() | setIds(List<Integer> ids) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "eventType": "primitive.variant",
  "ids": [
    77,
    78,
    79
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

