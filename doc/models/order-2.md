
# Order 2

Container for an individual order.

## Structure

`Order2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `OrderID` | `Integer` | Optional | Identifier of the order being shipped.<br><br>**Default**: `0` | Integer getOrderID() | setOrderID(Integer orderID) |
| `OrderNumber` | `String` | Optional | Number of the order being shipped. | String getOrderNumber() | setOrderNumber(String orderNumber) |
| `ReleaseNumber` | `String` | Optional | Release number of the order being shipped. | String getReleaseNumber() | setReleaseNumber(String releaseNumber) |
| `OrderReference1` | `String` | Optional | First order reference number. | String getOrderReference1() | setOrderReference1(String orderReference1) |
| `OrderReference2` | `String` | Optional | Second order reference number. | String getOrderReference2() | setOrderReference2(String orderReference2) |
| `OrderReference3` | `String` | Optional | Third order reference number. | String getOrderReference3() | setOrderReference3(String orderReference3) |
| `SalesOrderNumber` | `String` | Optional | Sales order number of the order being shipped. | String getSalesOrderNumber() | setSalesOrderNumber(String salesOrderNumber) |
| `PurchaseOrderNumber` | `String` | Optional | Purchase order number of the order being shipped. | String getPurchaseOrderNumber() | setPurchaseOrderNumber(String purchaseOrderNumber) |
| `RecordIdentifiers` | [`RecordIdentifiers3`](../../doc/models/record-identifiers-3.md) | Optional | Outer container for transaction identifiers. | RecordIdentifiers3 getRecordIdentifiers() | setRecordIdentifiers(RecordIdentifiers3 recordIdentifiers) |

## Example (as XML)

```xml
<wtg:Order xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:OrderID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:OrderID>
  <wtg:OrderNumber xmlns:wtg="https://www.wisetechglobal.com/">OrderNumber2</wtg:OrderNumber>
  <wtg:ReleaseNumber xmlns:wtg="https://www.wisetechglobal.com/">ReleaseNumber2</wtg:ReleaseNumber>
  <wtg:OrderReference1 xmlns:wtg="https://www.wisetechglobal.com/">OrderReference18</wtg:OrderReference1>
  <wtg:OrderReference2 xmlns:wtg="https://www.wisetechglobal.com/">OrderReference20</wtg:OrderReference2>
</wtg:Order>
```

