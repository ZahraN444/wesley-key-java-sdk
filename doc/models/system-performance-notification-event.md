
# System Performance Notification Event

*This model accepts additional fields of type Object.*

## Structure

`SystemPerformanceNotificationEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `SystemPerformanceNotificationEventType` | `String` | Required, Constant | **Value**: `"system.performance"` | String getSystemPerformanceNotificationEventType() | setSystemPerformanceNotificationEventType(String systemPerformanceNotificationEventType) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "systemPerformanceNotificationEventType": "system.performance",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

