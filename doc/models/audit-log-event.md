
# Audit Log Event

*This model accepts additional fields of type Object.*

## Structure

`AuditLogEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `EventType` | [`EventType3`](../../doc/models/event-type-3.md) | Optional | - | EventType3 getEventType() | setEventType(EventType3 eventType) |
| `Actor` | `String` | Optional | - | String getActor() | setActor(String actor) |
| `Action` | `String` | Optional | - | String getAction() | setAction(String action) |
| `Context` | `Object` | Optional | - | Object getContext() | setContext(Object context) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "eventType": "audit.log",
  "actor": "actor0",
  "action": "action2",
  "context": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

