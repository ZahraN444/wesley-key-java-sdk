
# Home Delivery

Container for home delivery details.

## Structure

`HomeDelivery`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | `Integer` | Optional | Type of home delivery required for the shipment. | Integer getType() | setType(Integer type) |
| `Date` | `String` | Optional | Date the shipment is to be home delivered. | String getDate() | setDate(String date) |
| `Phone` | `String` | Optional | The phone number associated with the address. | String getPhone() | setPhone(String phone) |
| `Signature` | `Boolean` | Optional | Indicates whether a signature is required prior to the package being released to the receiver.  Defaults to no signature required if not submitted.<br><br>**Default**: `false` | Boolean getSignature() | setSignature(Boolean signature) |

## Example (as XML)

```xml
<wtg:HomeDelivery xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Signature xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Signature>
  <wtg:Type xmlns:wtg="https://www.wisetechglobal.com/">140</wtg:Type>
  <wtg:Date xmlns:wtg="https://www.wisetechglobal.com/">Date6</wtg:Date>
  <wtg:Phone xmlns:wtg="https://www.wisetechglobal.com/">Phone0</wtg:Phone>
</wtg:HomeDelivery>
```

