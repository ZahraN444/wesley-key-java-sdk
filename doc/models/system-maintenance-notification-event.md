
# System Maintenance Notification Event

*This model accepts additional fields of type Object.*

## Structure

`SystemMaintenanceNotificationEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `SystemMaintenanceNotificationEventType` | `String` | Required, Constant | **Value**: `"system.maintenance"` | String getSystemMaintenanceNotificationEventType() | setSystemMaintenanceNotificationEventType(String systemMaintenanceNotificationEventType) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "systemMaintenanceNotificationEventType": "system.maintenance",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

