
# Charge 1

Container for an individual charge within the group associated with the transaction.

## Structure

`Charge1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ChargeType` | `String` | Optional | An identifier for the type of the charge. | String getChargeType() | setChargeType(String chargeType) |
| `ChargeDescription` | `String` | Optional | The description for the type of charge. | String getChargeDescription() | setChargeDescription(String chargeDescription) |
| `ChargeValue` | `String` | Optional | The value of the charge associated with the transaction. | String getChargeValue() | setChargeValue(String chargeValue) |
| `ChargeCurrency` | `String` | Optional | A code indicating the type of currency for the charge. | String getChargeCurrency() | setChargeCurrency(String chargeCurrency) |
| `ChargeISOCurrency` | `String` | Optional | International standard code for the charge group currency. | String getChargeISOCurrency() | setChargeISOCurrency(String chargeISOCurrency) |

## Example (as XML)

```xml
<wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ChargeType xmlns:wtg="https://www.wisetechglobal.com/">ChargeType2</wtg:ChargeType>
  <wtg:ChargeDescription xmlns:wtg="https://www.wisetechglobal.com/">ChargeDescription0</wtg:ChargeDescription>
  <wtg:ChargeValue xmlns:wtg="https://www.wisetechglobal.com/">ChargeValue0</wtg:ChargeValue>
  <wtg:ChargeCurrency xmlns:wtg="https://www.wisetechglobal.com/">ChargeCurrency0</wtg:ChargeCurrency>
  <wtg:ChargeISOCurrency xmlns:wtg="https://www.wisetechglobal.com/">ChargeISOCurrency2</wtg:ChargeISOCurrency>
</wtg:Charge>
```

