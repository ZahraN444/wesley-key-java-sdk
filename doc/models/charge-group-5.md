
# Charge Group 5

Container for an individual charge group associated with the transaction.

## Structure

`ChargeGroup5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ChargeGroupType` | `int` | Required | An identifier for the type of the charge group. | int getChargeGroupType() | setChargeGroupType(int chargeGroupType) |
| `ChargeGroupDescription` | `String` | Required | The description for the group of charges. | String getChargeGroupDescription() | setChargeGroupDescription(String chargeGroupDescription) |
| `ChargeGroupValue` | `Double` | Optional | The value of the charge group associated with the transaction.<br><br>**Default**: `0d` | Double getChargeGroupValue() | setChargeGroupValue(Double chargeGroupValue) |
| `ChargeGroupCurrency` | `String` | Optional | A code indicating the type of currency for the charges group. | String getChargeGroupCurrency() | setChargeGroupCurrency(String chargeGroupCurrency) |
| `ChargeGroupISOCurrency` | `Integer` | Optional | ISO code for the currency associated with the transaction.<br><br>**Default**: `0` | Integer getChargeGroupISOCurrency() | setChargeGroupISOCurrency(Integer chargeGroupISOCurrency) |
| `ChargeGroupISOCurrencySymbol` | `String` | Optional | Currency symbol for the charge group currency. | String getChargeGroupISOCurrencySymbol() | setChargeGroupISOCurrencySymbol(String chargeGroupISOCurrencySymbol) |
| `Charges` | [`Charges5`](../../doc/models/charges-5.md) | Required | Container for all charges within the group associated with the transaction. | Charges5 getCharges() | setCharges(Charges5 charges) |

## Example (as XML)

```xml
<wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ChargeGroupType xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroupType>
  <wtg:ChargeGroupDescription xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroupDescription>
  <wtg:ChargeGroupValue xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ChargeGroupValue>
  <wtg:ChargeGroupISOCurrency xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ChargeGroupISOCurrency>
  <wtg:Charges xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charges>
  <wtg:ChargeGroupCurrency xmlns:wtg="https://www.wisetechglobal.com/">ChargeGroupCurrency2</wtg:ChargeGroupCurrency>
  <wtg:ChargeGroupISOCurrencySymbol xmlns:wtg="https://www.wisetechglobal.com/">ChargeGroupISOCurrencySymbol2</wtg:ChargeGroupISOCurrencySymbol>
</wtg:ChargeGroup>
```

