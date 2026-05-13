
# Charge Groups 1

Container for all charge groups associated with the transaction.

## Structure

`ChargeGroups1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ChargeGroup` | [`List<ChargeGroup1>`](../../doc/models/charge-group-1.md) | Optional | Container for an individual charge group associated with the transaction. | List<ChargeGroup1> getChargeGroup() | setChargeGroup(List<ChargeGroup1> chargeGroup) |

## Example (as XML)

```xml
<wtg:ChargeGroups xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroup>
  <wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroup>
</wtg:ChargeGroups>
```

