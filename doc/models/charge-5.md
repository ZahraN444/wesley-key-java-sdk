
# Charge 5

Container for an individual charge within the group associated with the transaction.

## Structure

`Charge5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ChargeType` | `Integer` | Optional | An identifier for the type of the charge.<br><br>**Default**: `0` | Integer getChargeType() | setChargeType(Integer chargeType) |
| `ChargeDescription` | `String` | Optional | The description for the type of charge. | String getChargeDescription() | setChargeDescription(String chargeDescription) |
| `ChargeValue` | `Double` | Optional | The value of the charge associated with the transaction.<br><br>**Default**: `0d` | Double getChargeValue() | setChargeValue(Double chargeValue) |
| `ChargeCurrency` | `String` | Optional | A code indicating the type of currency for the charge. | String getChargeCurrency() | setChargeCurrency(String chargeCurrency) |
| `ChargeISOCurrency` | `Integer` | Optional | International standard code for the charge group currency.<br><br>**Default**: `0` | Integer getChargeISOCurrency() | setChargeISOCurrency(Integer chargeISOCurrency) |
| `ChargeExternalSystemCode` | `Integer` | Optional | A code to map to an external system.<br><br>**Default**: `0` | Integer getChargeExternalSystemCode() | setChargeExternalSystemCode(Integer chargeExternalSystemCode) |

## Example (as XML)

```xml
<wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ChargeType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ChargeType>
  <wtg:ChargeValue xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ChargeValue>
  <wtg:ChargeISOCurrency xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ChargeISOCurrency>
  <wtg:ChargeExternalSystemCode xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ChargeExternalSystemCode>
  <wtg:ChargeDescription xmlns:wtg="https://www.wisetechglobal.com/">ChargeDescription6</wtg:ChargeDescription>
  <wtg:ChargeCurrency xmlns:wtg="https://www.wisetechglobal.com/">ChargeCurrency6</wtg:ChargeCurrency>
</wtg:Charge>
```

