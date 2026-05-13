
# Rate 2

Container for individual rates associated with the package.

## Structure

`Rate2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RateType` | `String` | Optional | An identifier for the type of rate. | String getRateType() | setRateType(String rateType) |
| `TotalAccessorialCharges` | `String` | Optional | Total accessorial charge at package level for the rate type. | String getTotalAccessorialCharges() | setTotalAccessorialCharges(String totalAccessorialCharges) |
| `TotalShippingCharges` | `String` | Optional | Total shipping charge at package level for the rate type. | String getTotalShippingCharges() | setTotalShippingCharges(String totalShippingCharges) |
| `TotalCharges` | `String` | Optional | Total charge at package level for the rate type. | String getTotalCharges() | setTotalCharges(String totalCharges) |

## Example (as XML)

```xml
<wtg:Rate xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:RateType xmlns:wtg="https://www.wisetechglobal.com/">RateType8</wtg:RateType>
  <wtg:TotalAccessorialCharges xmlns:wtg="https://www.wisetechglobal.com/">TotalAccessorialCharges0</wtg:TotalAccessorialCharges>
  <wtg:TotalShippingCharges xmlns:wtg="https://www.wisetechglobal.com/">TotalShippingCharges6</wtg:TotalShippingCharges>
  <wtg:TotalCharges xmlns:wtg="https://www.wisetechglobal.com/">TotalCharges8</wtg:TotalCharges>
</wtg:Rate>
```

