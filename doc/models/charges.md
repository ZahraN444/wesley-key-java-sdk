
# Charges

Container for all charges within the group associated with the transaction.

## Structure

`Charges`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Charge` | [`List<Charge>`](../../doc/models/charge.md) | Optional | Container for an individual charge within the group associated with the transaction. | List<Charge> getCharge() | setCharge(List<Charge> charge) |

## Example (as XML)

```xml
<wtg:Charges xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Charge xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Charge>
</wtg:Charges>
```

