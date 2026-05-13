
# Charge

Container for an individual charge within the group associated with the transaction.

## Structure

`Charge`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ChargeType` | `int` | Required | An identifier for the type of the charge. | int getChargeType() | setChargeType(int chargeType) |
| `ChargeDescription` | `String` | Required | The description for the type of charge. | String getChargeDescription() | setChargeDescription(String chargeDescription) |
| `ChargeValue` | `double` | Required | The value of the charge associated with the transaction.<br><br>**Default**: `0d` | double getChargeValue() | setChargeValue(double chargeValue) |
| `ChargeCurrency` | `String` | Optional | A code indicating the type of currency for the charge. | String getChargeCurrency() | setChargeCurrency(String chargeCurrency) |
| `ChargeISOCurrency` | `Integer` | Optional | International standard code for the charge group currency.<br><br>**Default**: `0` | Integer getChargeISOCurrency() | setChargeISOCurrency(Integer chargeISOCurrency) |

## Example (as XML)

```xml
<wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ChargeType xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeType>
  <wtg:ChargeDescription xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeDescription>
  <wtg:ChargeValue xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ChargeValue>
  <wtg:ChargeISOCurrency xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ChargeISOCurrency>
  <wtg:ChargeCurrency xmlns:wtg="https://www.wisetechglobal.com/">ChargeCurrency2</wtg:ChargeCurrency>
</wtg:Charge>
```

