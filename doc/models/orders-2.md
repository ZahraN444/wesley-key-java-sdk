
# Orders 2

Container all orders associated with the transaction.

## Structure

`Orders2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Order` | [`List<Order2>`](../../doc/models/order-2.md) | Optional | Container for an individual order. | List<Order2> getOrder() | setOrder(List<Order2> order) |

## Example (as XML)

```xml
<wtg:Orders xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Order xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Order>
  <wtg:Order xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Order>
  <wtg:Order xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Order>
</wtg:Orders>
```

