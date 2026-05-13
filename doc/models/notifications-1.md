
# Notifications 1

Container for email notifications.

## Structure

`Notifications1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ReceiverShipmentNotification` | `Boolean` | Optional | Indicates the receiver should be notified when the shipment is shipped.<br><br>**Default**: `false` | Boolean getReceiverShipmentNotification() | setReceiverShipmentNotification(Boolean receiverShipmentNotification) |
| `SenderShipmentNotification` | `Boolean` | Optional | Indicates the sender should be notified when the shipment is shipped.<br><br>**Default**: `false` | Boolean getSenderShipmentNotification() | setSenderShipmentNotification(Boolean senderShipmentNotification) |
| `ShipmentNotificationDetail` | [`ShipmentNotificationDetail1`](../../doc/models/shipment-notification-detail-1.md) | Optional | Container for shipment notification deails. | ShipmentNotificationDetail1 getShipmentNotificationDetail() | setShipmentNotificationDetail(ShipmentNotificationDetail1 shipmentNotificationDetail) |
| `ReceiverDeliveryNotification` | `Boolean` | Optional | Indicates the receiver should be notified when the shipment is delivered.<br><br>**Default**: `false` | Boolean getReceiverDeliveryNotification() | setReceiverDeliveryNotification(Boolean receiverDeliveryNotification) |
| `SenderDeliveryNotification` | `Boolean` | Optional | Indicates the sender should be notified when the shipment is delivered.<br><br>**Default**: `false` | Boolean getSenderDeliveryNotification() | setSenderDeliveryNotification(Boolean senderDeliveryNotification) |
| `DeliveryNotificationDetail` | [`DeliveryNotificationDetail`](../../doc/models/delivery-notification-detail.md) | Optional | Container for shipment delivery notification deails. | DeliveryNotificationDetail getDeliveryNotificationDetail() | setDeliveryNotificationDetail(DeliveryNotificationDetail deliveryNotificationDetail) |
| `ReceiverExceptionNotification` | `Boolean` | Optional | Indicates the receiver should be notified if there is an issue with the shipment.<br><br>**Default**: `false` | Boolean getReceiverExceptionNotification() | setReceiverExceptionNotification(Boolean receiverExceptionNotification) |
| `SenderExceptionNotification` | `Boolean` | Optional | Indicates the sender should be notified if there is an issue with the shipment.<br><br>**Default**: `false` | Boolean getSenderExceptionNotification() | setSenderExceptionNotification(Boolean senderExceptionNotification) |
| `ExceptionNotificationDetail` | [`ExceptionNotificationDetail1`](../../doc/models/exception-notification-detail-1.md) | Optional | Container for shipment exception notification deails. | ExceptionNotificationDetail1 getExceptionNotificationDetail() | setExceptionNotificationDetail(ExceptionNotificationDetail1 exceptionNotificationDetail) |
| `OutForDeliveryNotificationDetail` | [`OutForDeliveryNotificationDetail`](../../doc/models/out-for-delivery-notification-detail.md) | Optional | Container for out for delivery email notification. | OutForDeliveryNotificationDetail getOutForDeliveryNotificationDetail() | setOutForDeliveryNotificationDetail(OutForDeliveryNotificationDetail outForDeliveryNotificationDetail) |
| `AtDepotNotificationDetail` | [`AtDepotNotificationDetail`](../../doc/models/at-depot-notification-detail.md) | Optional | Container for at depot email notifications. | AtDepotNotificationDetail getAtDepotNotificationDetail() | setAtDepotNotificationDetail(AtDepotNotificationDetail atDepotNotificationDetail) |
| `ReceiverOnTenderNotification` | `Boolean` | Optional | Indicates the receiver should be notified when the shipment is tendered.<br><br>**Default**: `false` | Boolean getReceiverOnTenderNotification() | setReceiverOnTenderNotification(Boolean receiverOnTenderNotification) |
| `SenderOnTenderNotification` | `Boolean` | Optional | Indicates the sender should be notified when the shipment is tendered.<br><br>**Default**: `false` | Boolean getSenderOnTenderNotification() | setSenderOnTenderNotification(Boolean senderOnTenderNotification) |
| `OnTenderNotificationDetail` | [`OnTenderNotificationDetail`](../../doc/models/on-tender-notification-detail.md) | Optional | Container for shipment tendering notification deails. | OnTenderNotificationDetail getOnTenderNotificationDetail() | setOnTenderNotificationDetail(OnTenderNotificationDetail onTenderNotificationDetail) |
| `PredictNotificationDetail` | [`PredictNotificationDetail`](../../doc/models/predict-notification-detail.md) | Optional | Container for predict email notifications. | PredictNotificationDetail getPredictNotificationDetail() | setPredictNotificationDetail(PredictNotificationDetail predictNotificationDetail) |
| `OtherShipmentNotifications` | `Boolean` | Optional | Indicates other should be notified when the shipment is shipped.<br><br>**Default**: `false` | Boolean getOtherShipmentNotifications() | setOtherShipmentNotifications(Boolean otherShipmentNotifications) |
| `OtherDeliveryNotifications` | `Boolean` | Optional | Indicates other should be notified when the shipment is delivered.<br><br>**Default**: `false` | Boolean getOtherDeliveryNotifications() | setOtherDeliveryNotifications(Boolean otherDeliveryNotifications) |
| `OtherExceptionNotifications` | `Boolean` | Optional | Indicates other should be notified if there is an issue with the shipment.<br><br>**Default**: `false` | Boolean getOtherExceptionNotifications() | setOtherExceptionNotifications(Boolean otherExceptionNotifications) |
| `OtherOnTenderNotifications` | `Boolean` | Optional | Indicates other should be notified when the shipment is tendered.<br><br>**Default**: `false` | Boolean getOtherOnTenderNotifications() | setOtherOnTenderNotifications(Boolean otherOnTenderNotifications) |
| `OtherNotificationDetail` | [`OtherNotificationDetail`](../../doc/models/other-notification-detail.md) | Optional | Container for other notification details. | OtherNotificationDetail getOtherNotificationDetail() | setOtherNotificationDetail(OtherNotificationDetail otherNotificationDetail) |
| `SenderPickupRequestConfirmationNotification` | `Boolean` | Optional | Indicates an email should be sent to the sender when a pickup request is received.<br><br>**Default**: `false` | Boolean getSenderPickupRequestConfirmationNotification() | setSenderPickupRequestConfirmationNotification(Boolean senderPickupRequestConfirmationNotification) |
| `SenderDriverOnRouteNotification` | `Boolean` | Optional | Indicates an email should be sent to the sender when a driver is on route to a pickup.<br><br>**Default**: `false` | Boolean getSenderDriverOnRouteNotification() | setSenderDriverOnRouteNotification(Boolean senderDriverOnRouteNotification) |
| `SenderPickupSecuredNotification` | `Boolean` | Optional | Indicates an email should be sent to the sender when a pickup has been loaded.<br><br>**Default**: `false` | Boolean getSenderPickupSecuredNotification() | setSenderPickupSecuredNotification(Boolean senderPickupSecuredNotification) |
| `SenderPickupExceptionNotification` | `Boolean` | Optional | Indicates an email should be sent to the sender when a pickup exception occurs.<br><br>**Default**: `false` | Boolean getSenderPickupExceptionNotification() | setSenderPickupExceptionNotification(Boolean senderPickupExceptionNotification) |
| `ReceiverPickupRequestConfirmationNotification` | `Boolean` | Optional | Indicates an email should be sent to the receiver when a pickup request is received.<br><br>**Default**: `false` | Boolean getReceiverPickupRequestConfirmationNotification() | setReceiverPickupRequestConfirmationNotification(Boolean receiverPickupRequestConfirmationNotification) |
| `ReceiverDriverOnRouteNotification` | `Boolean` | Optional | Indicates an email should be sent to the receiver when a driver is on route to a pickup.<br><br>**Default**: `false` | Boolean getReceiverDriverOnRouteNotification() | setReceiverDriverOnRouteNotification(Boolean receiverDriverOnRouteNotification) |
| `ReceiverPickupSecuredNotification` | `Boolean` | Optional | Indicates an email should be sent to the receiver when a pickup has been loaded.<br><br>**Default**: `false` | Boolean getReceiverPickupSecuredNotification() | setReceiverPickupSecuredNotification(Boolean receiverPickupSecuredNotification) |
| `ReceiverPickupExceptionNotification` | `Boolean` | Optional | Indicates an email should be sent to the receiver when a pickup exception occurs.<br><br>**Default**: `false` | Boolean getReceiverPickupExceptionNotification() | setReceiverPickupExceptionNotification(Boolean receiverPickupExceptionNotification) |
| `OtherPickupRequestConfirmationNotifications` | `Boolean` | Optional | Indicates an email should be sent to the addresses in the Other EMail Notifications Addresses when a pickup request is received.<br><br>**Default**: `false` | Boolean getOtherPickupRequestConfirmationNotifications() | setOtherPickupRequestConfirmationNotifications(Boolean otherPickupRequestConfirmationNotifications) |
| `OtherDriverOnRouteNotifications` | `Boolean` | Optional | Indicates an email should be sent to the addresses in the Other EMail Notifications Addresses when a driver is on route to a pickup.<br><br>**Default**: `false` | Boolean getOtherDriverOnRouteNotifications() | setOtherDriverOnRouteNotifications(Boolean otherDriverOnRouteNotifications) |
| `OtherPickupSecuredNotifications` | `Boolean` | Optional | Indicates an email should be sent to the addresses in the Other EMail Notifications Addresses when a pickup has been loaded.<br><br>**Default**: `false` | Boolean getOtherPickupSecuredNotifications() | setOtherPickupSecuredNotifications(Boolean otherPickupSecuredNotifications) |
| `OtherPickupExceptionNotifications` | `Boolean` | Optional | Indicates an email should be sent to the addresses in the Other EMail Notifications Addresses when a pickup exception occurs.<br><br>**Default**: `false` | Boolean getOtherPickupExceptionNotifications() | setOtherPickupExceptionNotifications(Boolean otherPickupExceptionNotifications) |

## Example (as XML)

```xml
<wtg:Notifications xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ReceiverShipmentNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReceiverShipmentNotification>
  <wtg:SenderShipmentNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SenderShipmentNotification>
  <wtg:ReceiverDeliveryNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReceiverDeliveryNotification>
  <wtg:SenderDeliveryNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SenderDeliveryNotification>
  <wtg:ReceiverExceptionNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReceiverExceptionNotification>
  <wtg:SenderExceptionNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SenderExceptionNotification>
  <wtg:ReceiverOnTenderNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReceiverOnTenderNotification>
  <wtg:SenderOnTenderNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SenderOnTenderNotification>
  <wtg:OtherShipmentNotifications xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OtherShipmentNotifications>
  <wtg:OtherDeliveryNotifications xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OtherDeliveryNotifications>
  <wtg:OtherExceptionNotifications xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OtherExceptionNotifications>
  <wtg:OtherOnTenderNotifications xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OtherOnTenderNotifications>
  <wtg:SenderPickupRequestConfirmationNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SenderPickupRequestConfirmationNotification>
  <wtg:SenderDriverOnRouteNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SenderDriverOnRouteNotification>
  <wtg:SenderPickupSecuredNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SenderPickupSecuredNotification>
  <wtg:SenderPickupExceptionNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SenderPickupExceptionNotification>
  <wtg:ReceiverPickupRequestConfirmationNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReceiverPickupRequestConfirmationNotification>
  <wtg:ReceiverDriverOnRouteNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReceiverDriverOnRouteNotification>
  <wtg:ReceiverPickupSecuredNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReceiverPickupSecuredNotification>
  <wtg:ReceiverPickupExceptionNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReceiverPickupExceptionNotification>
  <wtg:OtherPickupRequestConfirmationNotifications xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OtherPickupRequestConfirmationNotifications>
  <wtg:OtherDriverOnRouteNotifications xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OtherDriverOnRouteNotifications>
  <wtg:OtherPickupSecuredNotifications xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OtherPickupSecuredNotifications>
  <wtg:OtherPickupExceptionNotifications xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OtherPickupExceptionNotifications>
  <wtg:ShipmentNotificationDetail xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ShipmentNotificationDetail>
</wtg:Notifications>
```

