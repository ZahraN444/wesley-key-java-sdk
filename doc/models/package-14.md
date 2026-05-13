
# Package 14

Container for an individual package associated with the transaction.

## Structure

`Package14`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PackageID` | `Integer` | Optional | Unique identifier for the package.<br><br>**Default**: `0` | Integer getPackageID() | setPackageID(Integer packageID) |
| `PackageHistoryState` | `String` | Optional | Description of the package history status.<br><br>**Default**: `"0"` | String getPackageHistoryState() | setPackageHistoryState(String packageHistoryState) |
| `ShipperReference` | `String` | Optional | Primary shipping reference number. | String getShipperReference() | setShipperReference(String shipperReference) |
| `ReferenceOne` | `String` | Optional | First additional reference number. | String getReferenceOne() | setReferenceOne(String referenceOne) |
| `ReferenceTwo` | `String` | Optional | Second additional reference number. | String getReferenceTwo() | setReferenceTwo(String referenceTwo) |
| `ReferenceThree` | `String` | Optional | Third additional reference number. | String getReferenceThree() | setReferenceThree(String referenceThree) |
| `ReferenceFour` | `String` | Optional | Fourth additional reference number. | String getReferenceFour() | setReferenceFour(String referenceFour) |
| `ReferenceFive` | `String` | Optional | Fifth additional reference number. | String getReferenceFive() | setReferenceFive(String referenceFive) |
| `ReferenceSix` | `String` | Optional | Sixth additional reference number. | String getReferenceSix() | setReferenceSix(String referenceSix) |
| `WayBillNumber` | `String` | Optional | Tracking number of the package. | String getWayBillNumber() | setWayBillNumber(String wayBillNumber) |
| `RecordIdentifiers` | [`RecordIdentifiers7`](../../doc/models/record-identifiers-7.md) | Optional | Outer container for transaction identifiers. | RecordIdentifiers7 getRecordIdentifiers() | setRecordIdentifiers(RecordIdentifiers7 recordIdentifiers) |
| `International` | [`International12`](../../doc/models/international-12.md) | Optional | Container for international details associated with the shipment. | International12 getInternational() | setInternational(International12 international) |
| `Status` | [`Status6`](../../doc/models/status-6.md) | Required | Container for transaction errors and warning elements. | Status6 getStatus() | setStatus(Status6 status) |

## Example (as XML)

```xml
<wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:PackageID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageID>
  <wtg:PackageHistoryState xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageHistoryState>
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Status>
  <wtg:ShipperReference xmlns:wtg="https://www.wisetechglobal.com/">ShipperReference6</wtg:ShipperReference>
  <wtg:ReferenceOne xmlns:wtg="https://www.wisetechglobal.com/">ReferenceOne6</wtg:ReferenceOne>
  <wtg:ReferenceTwo xmlns:wtg="https://www.wisetechglobal.com/">ReferenceTwo2</wtg:ReferenceTwo>
</wtg:Package>
```

