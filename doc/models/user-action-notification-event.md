
# User Action Notification Event

*This model accepts additional fields of type Object.*

## Structure

`UserActionNotificationEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `UserActionNotificationEventType` | `String` | Required, Constant | **Value**: `"user.action"` | String getUserActionNotificationEventType() | setUserActionNotificationEventType(String userActionNotificationEventType) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "userActionNotificationEventType": "user.action",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

