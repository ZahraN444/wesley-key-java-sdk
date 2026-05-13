
# Personal Shipping 1

Container for personal shipping elements.

## Structure

`PersonalShipping1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PersonalShipment` | `Boolean` | Optional | Indicates that shipment is a personal shipment.<br><br>**Default**: `false` | Boolean getPersonalShipment() | setPersonalShipment(Boolean personalShipment) |
| `PaymentMethodID` | `String` | Optional | The id of the payment method used to pay for a personal shipment. | String getPaymentMethodID() | setPaymentMethodID(String paymentMethodID) |
| `PaymentIntentID` | `String` | Optional | The id of the payment intent used to pay for a personal shipment. | String getPaymentIntentID() | setPaymentIntentID(String paymentIntentID) |
| `TotalCharge` | `Double` | Optional | Cost that the customer will be charged for the personal shipment.<br><br>**Default**: `0d` | Double getTotalCharge() | setTotalCharge(Double totalCharge) |
| `ConvenienceFee` | `Double` | Optional | Cost to the user for processing a personal shipment. This cost is included in the total cost<br><br>**Default**: `0d` | Double getConvenienceFee() | setConvenienceFee(Double convenienceFee) |
| `SavePaymentMethod` | `Boolean` | Optional | Whether or not to save the payment method..<br><br>**Default**: `false` | Boolean getSavePaymentMethod() | setSavePaymentMethod(Boolean savePaymentMethod) |
| `UpdatePaymentMethod` | `Boolean` | Optional | Whether or not to update the payment method..<br><br>**Default**: `false` | Boolean getUpdatePaymentMethod() | setUpdatePaymentMethod(Boolean updatePaymentMethod) |
| `ExpMonth` | `Long` | Optional | The expiry month for the credit card. | Long getExpMonth() | setExpMonth(Long expMonth) |
| `ExpYear` | `Long` | Optional | The expiry year for the credit card. | Long getExpYear() | setExpYear(Long expYear) |
| `RequestEmailNotification` | `Boolean` | Optional | Request an email notification on successful shipment.<br><br>**Default**: `false` | Boolean getRequestEmailNotification() | setRequestEmailNotification(Boolean requestEmailNotification) |
| `Packages` | [`Packages7`](../../doc/models/packages-7.md) | Optional | Container for all packages associated with the transaction. | Packages7 getPackages() | setPackages(Packages7 packages) |

## Example (as XML)

```xml
<wtg:PersonalShipping xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:PersonalShipment xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PersonalShipment>
  <wtg:TotalCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TotalCharge>
  <wtg:ConvenienceFee xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ConvenienceFee>
  <wtg:SavePaymentMethod xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SavePaymentMethod>
  <wtg:UpdatePaymentMethod xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:UpdatePaymentMethod>
  <wtg:RequestEmailNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:RequestEmailNotification>
  <wtg:PaymentMethodID xmlns:wtg="https://www.wisetechglobal.com/">PaymentMethodID6</wtg:PaymentMethodID>
  <wtg:PaymentIntentID xmlns:wtg="https://www.wisetechglobal.com/">PaymentIntentID2</wtg:PaymentIntentID>
</wtg:PersonalShipping>
```

