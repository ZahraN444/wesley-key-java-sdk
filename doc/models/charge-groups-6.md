
# Charge Groups 6

Container for all charge groups associated with the transaction.

## Structure

`ChargeGroups6`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ChargeGroup` | [`List<ChargeGroup6>`](../../doc/models/charge-group-6.md) | Optional | Container for an individual charge group associated with the transaction. | List<ChargeGroup6> getChargeGroup() | setChargeGroup(List<ChargeGroup6> chargeGroup) |

## Example (as XML)

```xml
<wtg:ChargeGroups xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroup>
  <wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroup>
  <wtg:ChargeGroup xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroup>
</wtg:ChargeGroups>
```

