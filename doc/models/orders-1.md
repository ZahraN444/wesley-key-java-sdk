
# Orders 1

Container all orders associated with the transaction.

## Structure

`Orders1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Order` | [`List<Order1>`](../../doc/models/order-1.md) | Optional | Container for an individual order. | List<Order1> getOrder() | setOrder(List<Order1> order) |

## Example (as XML)

```xml
<wtg:Orders xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Order xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Order>
  <wtg:Order xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Order>
</wtg:Orders>
```

