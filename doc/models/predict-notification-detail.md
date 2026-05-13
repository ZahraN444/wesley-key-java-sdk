
# Predict Notification Detail

Container for predict email notifications.

## Structure

`PredictNotificationDetail`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `NotificationDeliveryMethod` | [`NotificationDeliveryMethodEnum`](../../doc/models/notification-delivery-method-enum.md) | Optional | The method that the notification will be sent. If it is not provided it is default to e-mail. | NotificationDeliveryMethodEnum getNotificationDeliveryMethod() | setNotificationDeliveryMethod(NotificationDeliveryMethodEnum notificationDeliveryMethod) |
| `Addresses` | `String` | Optional | Any additional email addresses / phone numbers that need to be sent to the carrier for the notifcations or key words RECEIVER / SENDER to pick the E-Mail / phone number from the data that is already entered. | String getAddresses() | setAddresses(String addresses) |

## Example (as XML)

```xml
<wtg:PredictNotificationDetail xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:NotificationDeliveryMethod xmlns:wtg="https://www.wisetechglobal.com/">1</wtg:NotificationDeliveryMethod>
  <wtg:Addresses xmlns:wtg="https://www.wisetechglobal.com/">Addresses4</wtg:Addresses>
</wtg:PredictNotificationDetail>
```

