
# User Status Notification Event

*This model accepts additional fields of type Object.*

## Structure

`UserStatusNotificationEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `UserStatusNotificationEventType` | `String` | Required, Constant | **Value**: `"user.status"` | String getUserStatusNotificationEventType() | setUserStatusNotificationEventType(String userStatusNotificationEventType) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "userStatusNotificationEventType": "user.status",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

