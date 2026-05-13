
# Package 11

Container for an individual package associated with the transaction.

## Structure

`Package11`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AccountID` | `Integer` | Optional | The account identifier that identifies the carrier account used for tracking.<br><br>**Default**: `0` | Integer getAccountID() | setAccountID(Integer accountID) |
| `PackageID` | `Integer` | Optional | Identifier of the package to track.  Must submit BoL number, package identifier or tracking number.<br><br>**Default**: `0` | Integer getPackageID() | setPackageID(Integer packageID) |
| `WayBillNumber` | `String` | Optional | Tracking number of the package to track.  Must submit BoL number, package identifier or tracking number. | String getWayBillNumber() | setWayBillNumber(String wayBillNumber) |
| `ShipperReference` | `String` | Optional | Track by Shipper reference number, supported by FedEx Web Services. | String getShipperReference() | setShipperReference(String shipperReference) |
| `ReferenceOne` | `String` | Optional | Track by reference number 1, supported by FedEx Web Services. | String getReferenceOne() | setReferenceOne(String referenceOne) |
| `ReferenceTwo` | `String` | Optional | Track by reference number 2, supported by FedEx Web Services. | String getReferenceTwo() | setReferenceTwo(String referenceTwo) |

## Example (as XML)

```xml
<wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:AccountID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:AccountID>
  <wtg:PackageID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageID>
  <wtg:WayBillNumber xmlns:wtg="https://www.wisetechglobal.com/">WayBillNumber8</wtg:WayBillNumber>
  <wtg:ShipperReference xmlns:wtg="https://www.wisetechglobal.com/">ShipperReference0</wtg:ShipperReference>
  <wtg:ReferenceOne xmlns:wtg="https://www.wisetechglobal.com/">ReferenceOne0</wtg:ReferenceOne>
</wtg:Package>
```

