
# Shipment Notification Detail 1

Container for shipment notification deails.

## Structure

`ShipmentNotificationDetail1`

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
<wtg:ShipmentNotificationDetail xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:NotificationDeliveryMethod xmlns:wtg="https://www.wisetechglobal.com/">1</wtg:NotificationDeliveryMethod>
  <wtg:Sender xmlns:wtg="https://www.wisetechglobal.com/">Sender6</wtg:Sender>
  <wtg:Subject xmlns:wtg="https://www.wisetechglobal.com/">Subject2</wtg:Subject>
  <wtg:Body xmlns:wtg="https://www.wisetechglobal.com/">Body4</wtg:Body>
  <wtg:Addresses xmlns:wtg="https://www.wisetechglobal.com/">Addresses8</wtg:Addresses>
</wtg:ShipmentNotificationDetail>
```

