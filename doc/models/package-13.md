
# Package 13

Container for an individual package associated with the transaction.

## Structure

`Package13`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PackageID` | `Integer` | Optional | Identifier of the package to void.  Must submit shipment identifier, shipment group identifier, package identifier or tracking number.<br><br>**Default**: `0` | Integer getPackageID() | setPackageID(Integer packageID) |
| `WayBillNumber` | `String` | Optional | Tracking Number of the package to void.  Must submit shipment identifier, shipment group identifier, package identifier or tracking number. | String getWayBillNumber() | setWayBillNumber(String wayBillNumber) |

## Example (as XML)

```xml
<wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:PackageID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageID>
  <wtg:WayBillNumber xmlns:wtg="https://www.wisetechglobal.com/">WayBillNumber8</wtg:WayBillNumber>
</wtg:Package>
```

