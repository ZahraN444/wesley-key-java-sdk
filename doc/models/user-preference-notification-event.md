
# User Preference Notification Event

*This model accepts additional fields of type Object.*

## Structure

`UserPreferenceNotificationEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `UserPreferenceNotificationEventType` | `String` | Required, Constant | **Value**: `"user.preference"` | String getUserPreferenceNotificationEventType() | setUserPreferenceNotificationEventType(String userPreferenceNotificationEventType) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "userPreferenceNotificationEventType": "user.preference",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

