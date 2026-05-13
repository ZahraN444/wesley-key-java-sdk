
# Charges 6

Container for all charges within the group associated with the transaction.

## Structure

`Charges6`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Charge` | [`List<Charge6>`](../../doc/models/charge-6.md) | Optional | Container for an individual charge within the group associated with the transaction. | List<Charge6> getCharge() | setCharge(List<Charge6> charge) |

## Example (as XML)

```xml
<wtg:Charges xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charge>
  <wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charge>
  <wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charge>
</wtg:Charges>
```

