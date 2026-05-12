
# Notification Callback

*This model accepts additional fields of type Object.*

## Structure

`NotificationCallback`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `NotificationType` | `String` | Required | - | String getNotificationType() | setNotificationType(String notificationType) |
| `Subject` | `String` | Required | - | String getSubject() | setSubject(String subject) |
| `Message` | `String` | Required | - | String getMessage() | setMessage(String message) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "notificationType": "email",
  "subject": "Order Coonfirmation",
  "message": "msg_email_789",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

