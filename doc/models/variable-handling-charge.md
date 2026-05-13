
# Variable Handling Charge

Container for variable handling charge elements.

## Structure

`VariableHandlingCharge`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RateType` | `Integer` | Optional | Rate type to apply handling charge to. 1 = Account Rates; 2 = List Rates<br><br>**Constraints**: *Pattern*: `[1-2]` | Integer getRateType() | setRateType(Integer rateType) |
| `RateBasis` | `Integer` | Optional | Charge basis upon which the handling charge is calculated. 1 = Base Charge; 2 = Net Charge; 3 = Net Charge Excluding Taxes; 4 = Net Freight<br><br>**Constraints**: *Pattern*: `[1-4]` | Integer getRateBasis() | setRateBasis(Integer rateBasis) |
| `FixedValue` | `Double` | Optional | Fixed value of handling charge.<br><br>**Default**: `0d` | Double getFixedValue() | setFixedValue(Double fixedValue) |
| `PercentageValue` | `Double` | Optional | Percentage value of handling charge.<br><br>**Default**: `0d` | Double getPercentageValue() | setPercentageValue(Double percentageValue) |

## Example (as XML)

```xml
<wtg:VariableHandlingCharge xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:FixedValue xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:FixedValue>
  <wtg:PercentageValue xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PercentageValue>
  <wtg:RateType xmlns:wtg="https://www.wisetechglobal.com/">56</wtg:RateType>
  <wtg:RateBasis xmlns:wtg="https://www.wisetechglobal.com/">96</wtg:RateBasis>
</wtg:VariableHandlingCharge>
```

