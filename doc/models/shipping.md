
# Shipping

Container for shipping associated with the transaction.

## Structure

`Shipping`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ShippingCharge` | `double` | Required | The total cost for all shipping related charges.<br><br>**Default**: `0d` | double getShippingCharge() | setShippingCharge(double shippingCharge) |
| `AccessorialCharge` | `double` | Required | The total for all accessorial shipping related charges.<br><br>**Default**: `0d` | double getAccessorialCharge() | setAccessorialCharge(double accessorialCharge) |
| `OtherCharge` | `double` | Required | The total for any charges not covered by other shipping totals.<br><br>**Default**: `0d` | double getOtherCharge() | setOtherCharge(double otherCharge) |
| `TotalCharge` | `double` | Required | The total charge for all shipping related charges.<br><br>**Default**: `0d` | double getTotalCharge() | setTotalCharge(double totalCharge) |
| `NetRate` | `double` | Required | The total for all shipping net charges.<br><br>**Default**: `0d` | double getNetRate() | setNetRate(double netRate) |
| `Currency` | `String` | Optional | The currency code associated with the transaction. | String getCurrency() | setCurrency(String currency) |
| `ISOCurrency` | `Integer` | Optional | The ID of the ISO currency used.<br><br>**Default**: `0` | Integer getISOCurrency() | setISOCurrency(Integer iSOCurrency) |

## Example (as XML)

```xml
<wtg:Shipping xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ShippingCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ShippingCharge>
  <wtg:AccessorialCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:AccessorialCharge>
  <wtg:OtherCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:OtherCharge>
  <wtg:TotalCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TotalCharge>
  <wtg:NetRate xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:NetRate>
  <wtg:ISOCurrency xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ISOCurrency>
  <wtg:Currency xmlns:wtg="https://www.wisetechglobal.com/">Currency0</wtg:Currency>
</wtg:Shipping>
```

