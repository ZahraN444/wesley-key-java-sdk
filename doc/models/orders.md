
# Orders

Container all orders associated with the transaction.

## Structure

`Orders`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Order` | [`List<Order>`](../../doc/models/order.md) | Optional | Container for an individual order. | List<Order> getOrder() | setOrder(List<Order> order) |

## Example (as XML)

```xml
<wtg:Orders xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Order xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Order>
</wtg:Orders>
```

