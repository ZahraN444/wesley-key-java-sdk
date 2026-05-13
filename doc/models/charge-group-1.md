
# Charge Group 1

Container for an individual charge group associated with the transaction.

## Structure

`ChargeGroup1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ChargeGroupType` | `String` | Optional | An identifier for the type of the charge group. | String getChargeGroupType() | setChargeGroupType(String chargeGroupType) |
| `ChargeGroupDescription` | `String` | Optional | The description for the group of charges. | String getChargeGroupDescription() | setChargeGroupDescription(String chargeGroupDescription) |
| `ChargeGroupValue` | `String` | Optional | The value of the charge group associated with the transaction. | String getChargeGroupValue() | setChargeGroupValue(String chargeGroupValue) |
| `ChargeGroupCurrency` | `String` | Optional | A code indicating the type of currency for the charges group. | String getChargeGroupCurrency() | setChargeGroupCurrency(String chargeGroupCurrency) |
| `ChargeGroupISOCurrency` | `String` | Optional | ISO code for the currency associated with the transaction. | String getChargeGroupISOCurrency() | setChargeGroupISOCurrency(String chargeGroupISOCurrency) |
| `ChargeGroupISOCurrencySymbol` | `String` | Optional | Currency symbol for the charge group currency. | String getChargeGroupISOCurrencySymbol() | setChargeGroupISOCurrencySymbol(String chargeGroupISOCurrencySymbol) |
| `Charges` | [`Charges1`](../../doc/models/charges-1.md) | Required | Container for all charges within the group associated with the transaction. | Charges1 getCharges() | setCharges(Charges1 charges) |

## Example (as XML)

```xml
<wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ChargeGroupType xmlns:wtg="https://www.wisetechglobal.com/">ChargeGroupType2</wtg:ChargeGroupType>
  <wtg:ChargeGroupDescription xmlns:wtg="https://www.wisetechglobal.com/">ChargeGroupDescription4</wtg:ChargeGroupDescription>
  <wtg:ChargeGroupValue xmlns:wtg="https://www.wisetechglobal.com/">ChargeGroupValue8</wtg:ChargeGroupValue>
  <wtg:ChargeGroupCurrency xmlns:wtg="https://www.wisetechglobal.com/">ChargeGroupCurrency0</wtg:ChargeGroupCurrency>
  <wtg:ChargeGroupISOCurrency xmlns:wtg="https://www.wisetechglobal.com/">ChargeGroupISOCurrency0</wtg:ChargeGroupISOCurrency>
  <wtg:Charges xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charges>
</wtg:ChargeGroup>
```

