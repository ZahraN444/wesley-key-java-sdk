
# On Tender Notification Detail

Container for shipment tendering notification deails.

## Structure

`OnTenderNotificationDetail`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Sender` | `String` | Optional | The name of the notification sender. Defaults to shipper company name if not submitted. | String getSender() | setSender(String sender) |
| `Subject` | `String` | Optional | The subject line for the notification. Defaults to carrier default if not submitted. | String getSubject() | setSubject(String subject) |
| `Body` | `String` | Optional | The body of the notification sent. Defaults to carrier default text if not submitted. | String getBody() | setBody(String body) |
| `Addresses` | `String` | Optional | Any additional email addresses that need to be sent to the carrier for the notifcations. | String getAddresses() | setAddresses(String addresses) |

## Example (as XML)

```xml
<wtg:OnTenderNotificationDetail xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Sender xmlns:wtg="https://www.wisetechglobal.com/">Sender0</wtg:Sender>
  <wtg:Subject xmlns:wtg="https://www.wisetechglobal.com/">Subject8</wtg:Subject>
  <wtg:Body xmlns:wtg="https://www.wisetechglobal.com/">Body8</wtg:Body>
  <wtg:Addresses xmlns:wtg="https://www.wisetechglobal.com/">Addresses2</wtg:Addresses>
</wtg:OnTenderNotificationDetail>
```

