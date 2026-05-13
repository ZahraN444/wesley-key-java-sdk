
# Personal Shipping 2

Container for personal shipping elements.

## Structure

`PersonalShipping2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PersonalShipment` | `Boolean` | Optional | Indicates that shipment is a personal shipment.<br><br>**Default**: `false` | Boolean getPersonalShipment() | setPersonalShipment(Boolean personalShipment) |
| `PaymentIntentID` | `String` | Optional | The id of the payment intent used to pay for a personal shipment. | String getPaymentIntentID() | setPaymentIntentID(String paymentIntentID) |
| `TotalCharge` | `Double` | Optional | Cost that the customer will be charged for the personal shipment.<br><br>**Default**: `0d` | Double getTotalCharge() | setTotalCharge(Double totalCharge) |
| `ConvenienceFee` | `Double` | Optional | Cost to the user for processing a personal shipment. This cost is included in the total cost<br><br>**Default**: `0d` | Double getConvenienceFee() | setConvenienceFee(Double convenienceFee) |
| `PaymentStatus` | [`PaymentStatus`](../../doc/models/payment-status.md) | Optional | Container for payment processing status. | PaymentStatus getPaymentStatus() | setPaymentStatus(PaymentStatus paymentStatus) |

## Example (as XML)

```xml
<wtg:PersonalShipping xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:PersonalShipment xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PersonalShipment>
  <wtg:TotalCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TotalCharge>
  <wtg:ConvenienceFee xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ConvenienceFee>
  <wtg:PaymentIntentID xmlns:wtg="https://www.wisetechglobal.com/">PaymentIntentID8</wtg:PaymentIntentID>
  <wtg:PaymentStatus xmlns:wtg="https://www.wisetechglobal.com/"></wtg:PaymentStatus>
</wtg:PersonalShipping>
```

