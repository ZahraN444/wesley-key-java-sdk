
# Charges 5

Container for all charges within the group associated with the transaction.

## Structure

`Charges5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Charge` | [`List<Charge5>`](../../doc/models/charge-5.md) | Optional | Container for an individual charge within the group associated with the transaction. | List<Charge5> getCharge() | setCharge(List<Charge5> charge) |

## Example (as XML)

```xml
<wtg:Charges xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charge>
</wtg:Charges>
```

