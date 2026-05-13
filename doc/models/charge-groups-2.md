
# Charge Groups 2

Container for all charge groups associated with the transaction.

## Structure

`ChargeGroups2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ChargeGroup` | [`List<ChargeGroup2>`](../../doc/models/charge-group-2.md) | Optional | Container for an individual charge group associated with the transaction. | List<ChargeGroup2> getChargeGroup() | setChargeGroup(List<ChargeGroup2> chargeGroup) |

## Example (as XML)

```xml
<wtg:ChargeGroups xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroup>
  <wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroup>
</wtg:ChargeGroups>
```

