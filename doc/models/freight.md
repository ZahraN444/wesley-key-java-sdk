
# Freight

Container for freight specific values

## Structure

`Freight`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Billing` | [`Billing1`](../../doc/models/billing-1.md) | Optional | Container for billing details associated with the transaction. | Billing1 getBilling() | setBilling(Billing1 billing) |

## Example (as XML)

```xml
<wtg:Freight xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Billing xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Billing>
</wtg:Freight>
```

