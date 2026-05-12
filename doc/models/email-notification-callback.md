
# Email Notification Callback

*This model accepts additional fields of type Object.*

## Structure

`EmailNotificationCallback`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `MessageId` | `String` | Optional | - | String getMessageId() | setMessageId(String messageId) |
| `RecipientEmail` | `String` | Optional | - | String getRecipientEmail() | setRecipientEmail(String recipientEmail) |
| `Status` | [`Status1`](../../doc/models/status-1.md) | Optional | - | Status1 getStatus() | setStatus(Status1 status) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "messageId": "msg_001",
  "recipientEmail": "user@example.com",
  "status": "sent",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

