
# Rate 7

Container for an individual rate.

## Structure

`Rate7`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RateType` | `int` | Required | Numeric identifier for the rate type. | int getRateType() | setRateType(int rateType) |
| `TotalAccessorialCharges` | `Double` | Optional | Total accessorial charges for the rate type. | Double getTotalAccessorialCharges() | setTotalAccessorialCharges(Double totalAccessorialCharges) |
| `TotalShippingCharges` | `Double` | Optional | Total shipping charges for the rate type. | Double getTotalShippingCharges() | setTotalShippingCharges(Double totalShippingCharges) |
| `TotalCharges` | `Double` | Optional | Total packages charge for the rate type. | Double getTotalCharges() | setTotalCharges(Double totalCharges) |

## Example (as XML)

```xml
<wtg:Rate xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:RateType xmlns:wtg="https://www.wisetechglobal.com/">252</wtg:RateType>
  <wtg:TotalAccessorialCharges xmlns:wtg="https://www.wisetechglobal.com/">20.56</wtg:TotalAccessorialCharges>
  <wtg:TotalShippingCharges xmlns:wtg="https://www.wisetechglobal.com/">86.7</wtg:TotalShippingCharges>
  <wtg:TotalCharges xmlns:wtg="https://www.wisetechglobal.com/">8.34</wtg:TotalCharges>
</wtg:Rate>
```

