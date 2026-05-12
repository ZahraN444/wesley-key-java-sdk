
# Sms Notification Callback

*This model accepts additional fields of type Object.*

## Structure

`SmsNotificationCallback`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `MessageId` | `String` | Optional | - | String getMessageId() | setMessageId(String messageId) |
| `PhoneNumber` | `String` | Optional | - | String getPhoneNumber() | setPhoneNumber(String phoneNumber) |
| `Status` | [`Status2`](../../doc/models/status-2.md) | Optional | - | Status2 getStatus() | setStatus(Status2 status) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "messageId": "sms_002",
  "phoneNumber": "+15551234567",
  "status": "delivered",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

