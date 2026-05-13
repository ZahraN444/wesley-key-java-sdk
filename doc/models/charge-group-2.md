
# Charge Group 2

Container for an individual charge group associated with the transaction.

## Structure

`ChargeGroup2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ChargeGroupType` | `Integer` | Optional | An identifier for the type of the charge group.<br><br>**Default**: `0` | Integer getChargeGroupType() | setChargeGroupType(Integer chargeGroupType) |
| `ChargeGroupDescription` | `String` | Optional | The description for the group of charges. | String getChargeGroupDescription() | setChargeGroupDescription(String chargeGroupDescription) |
| `ChargeGroupValue` | `Double` | Optional | The value of the charge group associated with the transaction.<br><br>**Default**: `0d` | Double getChargeGroupValue() | setChargeGroupValue(Double chargeGroupValue) |
| `ChargeGroupCurrency` | `String` | Optional | A code indicating the type of currency for the charges group. | String getChargeGroupCurrency() | setChargeGroupCurrency(String chargeGroupCurrency) |
| `Charges` | [`Charges2`](../../doc/models/charges-2.md) | Required | Container for all charges within the group associated with the transaction. | Charges2 getCharges() | setCharges(Charges2 charges) |

## Example (as XML)

```xml
<wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ChargeGroupType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ChargeGroupType>
  <wtg:ChargeGroupValue xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ChargeGroupValue>
  <wtg:Charges xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charges>
  <wtg:ChargeGroupDescription xmlns:wtg="https://www.wisetechglobal.com/">ChargeGroupDescription4</wtg:ChargeGroupDescription>
  <wtg:ChargeGroupCurrency xmlns:wtg="https://www.wisetechglobal.com/">ChargeGroupCurrency0</wtg:ChargeGroupCurrency>
</wtg:ChargeGroup>
```

