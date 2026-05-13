
# Customer

Container for customer details.

## Structure

`Customer`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ShippingCharge` | `Double` | Optional | The total cost for all customer related charges.<br><br>**Default**: `0d` | Double getShippingCharge() | setShippingCharge(Double shippingCharge) |
| `AccessorialCharge` | `Double` | Optional | The total for all accessorial customer related charges.<br><br>**Default**: `0d` | Double getAccessorialCharge() | setAccessorialCharge(Double accessorialCharge) |
| `OtherCharge` | `Double` | Optional | The total for any charges not covered by other customer totals.<br><br>**Default**: `0d` | Double getOtherCharge() | setOtherCharge(Double otherCharge) |
| `TotalCharge` | `Double` | Optional | The total charge for all customer related charges.<br><br>**Default**: `0d` | Double getTotalCharge() | setTotalCharge(Double totalCharge) |
| `NetRate` | `Double` | Optional | The total for all customer net charges.<br><br>**Default**: `0d` | Double getNetRate() | setNetRate(Double netRate) |
| `Currency` | `String` | Optional | The currency code associated with the transaction. | String getCurrency() | setCurrency(String currency) |
| `ISOCurrency` | `Integer` | Optional | The ID of the ISO currency used.<br><br>**Default**: `0` | Integer getISOCurrency() | setISOCurrency(Integer iSOCurrency) |

## Example (as XML)

```xml
<wtg:Customer xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ShippingCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ShippingCharge>
  <wtg:AccessorialCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:AccessorialCharge>
  <wtg:OtherCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:OtherCharge>
  <wtg:TotalCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TotalCharge>
  <wtg:NetRate xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:NetRate>
  <wtg:ISOCurrency xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ISOCurrency>
</wtg:Customer>
```

