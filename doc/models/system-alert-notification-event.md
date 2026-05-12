
# System Alert Notification Event

*This model accepts additional fields of type Object.*

## Structure

`SystemAlertNotificationEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `SystemAlertNotificationEventType` | `String` | Required, Constant | **Value**: `"system.alert"` | String getSystemAlertNotificationEventType() | setSystemAlertNotificationEventType(String systemAlertNotificationEventType) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "systemAlertNotificationEventType": "system.alert",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

