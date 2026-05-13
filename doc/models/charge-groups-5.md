
# Charge Groups 5

Container for all charge groups associated with the transaction.

## Structure

`ChargeGroups5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ChargeGroup` | [`List<ChargeGroup5>`](../../doc/models/charge-group-5.md) | Optional | Container for an individual charge group associated with the transaction. | List<ChargeGroup5> getChargeGroup() | setChargeGroup(List<ChargeGroup5> chargeGroup) |

## Example (as XML)

```xml
<wtg:ChargeGroups xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroup>
  <wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroup>
  <wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroup>
</wtg:ChargeGroups>
```

