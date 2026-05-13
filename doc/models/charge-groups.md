
# Charge Groups

Container for all charge groups associated with the transaction.

## Structure

`ChargeGroups`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ChargeGroup` | [`List<ChargeGroup>`](../../doc/models/charge-group.md) | Optional | Container for an individual charge group associated with the transaction. | List<ChargeGroup> getChargeGroup() | setChargeGroup(List<ChargeGroup> chargeGroup) |

## Example (as XML)

```xml
<wtg:ChargeGroups xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroup>
</wtg:ChargeGroups>
```

