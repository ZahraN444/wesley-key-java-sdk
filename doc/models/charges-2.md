
# Charges 2

Container for all charges within the group associated with the transaction.

## Structure

`Charges2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Charge` | [`List<Charge2>`](../../doc/models/charge-2.md) | Optional | Container for an individual charge within the group associated with the transaction. | List<Charge2> getCharge() | setCharge(List<Charge2> charge) |

## Example (as XML)

```xml
<wtg:Charges xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charge>
  <wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charge>
  <wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charge>
</wtg:Charges>
```

