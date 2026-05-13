
# Insurance

Container for insurance details.

## Structure

`Insurance`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | `Integer` | Optional | Type of insurance.  Defaults to no insurance if not submitted.<br><br>**Default**: `0` | Integer getType() | setType(Integer type) |
| `Value` | `Double` | Optional | Value the package is to be insured for.<br><br>**Default**: `0d` | Double getValue() | setValue(Double value) |
| `ValueCurrency` | `String` | Optional | Currency of the value the package is to be insured for. | String getValueCurrency() | setValueCurrency(String valueCurrency) |

## Example (as XML)

```xml
<wtg:Insurance xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Type xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Type>
  <wtg:Value xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Value>
  <wtg:ValueCurrency xmlns:wtg="https://www.wisetechglobal.com/">ValueCurrency4</wtg:ValueCurrency>
</wtg:Insurance>
```

