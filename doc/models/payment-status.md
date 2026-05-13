
# Payment Status

Container for payment processing status.

## Structure

`PaymentStatus`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Status` | `String` | Required | Status of this PaymentIntent, one of requires_payment_method, requires_confirmation, requires_action, processing, requires_capture, canceled, or succeeded. | String getStatus() | setStatus(String status) |
| `PaymentIntentClientID` | `String` | Optional | Unique identifier for a payment assigned by payment handler for 3d auth. | String getPaymentIntentClientID() | setPaymentIntentClientID(String paymentIntentClientID) |
| `Action` | [`Action`](../../doc/models/action.md) | Optional | If present, this property tells you what actions you need to take in order for your customer to fulfill a payment using the provided source. | Action getAction() | setAction(Action action) |

## Example (as XML)

```xml
<wtg:PaymentStatus xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/">Status6</wtg:Status>
  <wtg:PaymentIntentClientID xmlns:wtg="https://www.wisetechglobal.com/">PaymentIntentClientID2</wtg:PaymentIntentClientID>
  <wtg:Action xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Action>
</wtg:PaymentStatus>
```

