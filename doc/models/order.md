
# Order

Container for an individual order.

## Structure

`Order`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `OrderID` | `Integer` | Optional | Identifier of the order being rated.<br><br>**Default**: `0` | Integer getOrderID() | setOrderID(Integer orderID) |
| `PickLists` | [`PickLists`](../../doc/models/pick-lists.md) | Optional | Container all order picklists. | PickLists getPickLists() | setPickLists(PickLists pickLists) |
| `OrderNumber` | `String` | Optional | Order number of the order being rated. | String getOrderNumber() | setOrderNumber(String orderNumber) |

## Example (as XML)

```xml
<wtg:Order xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:OrderID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:OrderID>
  <wtg:PickLists xmlns:wtg="https://www.wisetechglobal.com/"></wtg:PickLists>
  <wtg:OrderNumber xmlns:wtg="https://www.wisetechglobal.com/">OrderNumber8</wtg:OrderNumber>
</wtg:Order>
```

