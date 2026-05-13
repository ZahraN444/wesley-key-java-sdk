
# Exception Notification Detail 1

Container for shipment exception notification deails.

## Structure

`ExceptionNotificationDetail1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `NotificationDeliveryMethod` | [`NotificationDeliveryMethodEnum`](../../doc/models/notification-delivery-method-enum.md) | Optional | The method by which the notification will be sent. | NotificationDeliveryMethodEnum getNotificationDeliveryMethod() | setNotificationDeliveryMethod(NotificationDeliveryMethodEnum notificationDeliveryMethod) |
| `Sender` | `String` | Optional | The name of the notification sender. Defaults to shipper company name if not submitted. | String getSender() | setSender(String sender) |
| `Subject` | `String` | Optional | The subject line for the notification. Defaults to carrier default if not submitted. | String getSubject() | setSubject(String subject) |
| `Body` | `String` | Optional | The body of the notification sent. Defaults to carrier default text if not submitted. | String getBody() | setBody(String body) |
| `Addresses` | `String` | Optional | Any email addresses / phone numbers that need to be sent to the carrier for the notifcations or key words RECEIVER / SENDER to pick the E-Mail / phone number from the data that is already entered. | String getAddresses() | setAddresses(String addresses) |

## Example (as XML)

```xml
<wtg:ExceptionNotificationDetail xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:NotificationDeliveryMethod xmlns:wtg="https://www.wisetechglobal.com/">2</wtg:NotificationDeliveryMethod>
  <wtg:Sender xmlns:wtg="https://www.wisetechglobal.com/">Sender2</wtg:Sender>
  <wtg:Subject xmlns:wtg="https://www.wisetechglobal.com/">Subject6</wtg:Subject>
  <wtg:Body xmlns:wtg="https://www.wisetechglobal.com/">Body0</wtg:Body>
  <wtg:Addresses xmlns:wtg="https://www.wisetechglobal.com/">Addresses4</wtg:Addresses>
</wtg:ExceptionNotificationDetail>
```

