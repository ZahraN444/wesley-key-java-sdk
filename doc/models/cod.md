
# COD

Container for collect on delivery details.

## Structure

`COD`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | `Integer` | Optional | Numeric identifer for the type of cash on delivery.  Defaults to no cash on delivery if not submitted.<br><br>**Constraints**: *Pattern*: `[1-6]` | Integer getType() | setType(Integer type) |
| `Value` | `Double` | Optional | Value that is to be collected by the carrier when the package is delivered.<br><br>**Default**: `0d` | Double getValue() | setValue(Double value) |
| `ValueCurrency` | `String` | Optional | Currency of the value that is to be collected by the carrier when the package is delivered. | String getValueCurrency() | setValueCurrency(String valueCurrency) |
| `AddCharges` | `Boolean` | Optional | Indicates whether charges are to be added.<br><br>**Default**: `false` | Boolean getAddCharges() | setAddCharges(Boolean addCharges) |

## Example (as XML)

```xml
<wtg:COD xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Value xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Value>
  <wtg:AddCharges xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AddCharges>
  <wtg:Type xmlns:wtg="https://www.wisetechglobal.com/">226</wtg:Type>
  <wtg:ValueCurrency xmlns:wtg="https://www.wisetechglobal.com/">ValueCurrency2</wtg:ValueCurrency>
</wtg:COD>
```

