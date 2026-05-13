
# Charges 1

Container for all charges within the group associated with the transaction.

## Structure

`Charges1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Charge` | [`List<Charge1>`](../../doc/models/charge-1.md) | Optional | Container for an individual charge within the group associated with the transaction. | List<Charge1> getCharge() | setCharge(List<Charge1> charge) |

## Example (as XML)

```xml
<wtg:Charges xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charge>
  <wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charge>
</wtg:Charges>
```

