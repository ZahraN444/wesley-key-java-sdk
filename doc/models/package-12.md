
# Package 12

Container for an individual package associated with the transaction.

## Structure

`Package12`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Status` | [`Status5`](../../doc/models/status-5.md) | Required | Container for transaction errors and warning elements. | Status5 getStatus() | setStatus(Status5 status) |
| `History` | [`History`](../../doc/models/history.md) | Optional | Container for the package history status entries. | History getHistory() | setHistory(History history) |
| `PackageID` | `Integer` | Optional | Unique identifier for the package. | Integer getPackageID() | setPackageID(Integer packageID) |
| `Weight` | `Double` | Optional | The weight of the package.<br><br>**Default**: `0d` | Double getWeight() | setWeight(Double weight) |
| `WayBillNumber` | `String` | Optional | Tracking number of the package. | String getWayBillNumber() | setWayBillNumber(String wayBillNumber) |
| `ShipperReference` | `String` | Optional | Primary shipping reference number. | String getShipperReference() | setShipperReference(String shipperReference) |
| `ReferenceOne` | `String` | Optional | First additional reference number. | String getReferenceOne() | setReferenceOne(String referenceOne) |
| `ReferenceTwo` | `String` | Optional | Second additional reference number. | String getReferenceTwo() | setReferenceTwo(String referenceTwo) |
| `ReferenceThree` | `String` | Optional | Third additional reference number. | String getReferenceThree() | setReferenceThree(String referenceThree) |
| `ReferenceFour` | `String` | Optional | Fourth additional reference number. | String getReferenceFour() | setReferenceFour(String referenceFour) |
| `ReferenceFive` | `String` | Optional | Fifth additional reference number. | String getReferenceFive() | setReferenceFive(String referenceFive) |
| `ReferenceSix` | `String` | Optional | Sixth additional reference number. | String getReferenceSix() | setReferenceSix(String referenceSix) |
| `PackageType` | `Integer` | Optional | Unique identifier of the package type associated with the package.<br><br>**Default**: `0` | Integer getPackageType() | setPackageType(Integer packageType) |
| `PackageTypeName` | `String` | Optional | Carrier package type (e.g. letter, package, pallet) associated with the package.<br><br>**Default**: `"0"` | String getPackageTypeName() | setPackageTypeName(String packageTypeName) |
| `ReceiverName` | `String` | Optional | The name of for the receiver of the package. | String getReceiverName() | setReceiverName(String receiverName) |
| `ReceiverPhone` | `String` | Optional | The phone number for the receiver of the package. | String getReceiverPhone() | setReceiverPhone(String receiverPhone) |
| `ReceiverEmail` | `String` | Optional | The email address for the receiver of the package. | String getReceiverEmail() | setReceiverEmail(String receiverEmail) |

## Example (as XML)

```xml
<wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Status>
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Weight>
  <wtg:PackageType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageType>
  <wtg:PackageTypeName xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageTypeName>
  <wtg:History xmlns:wtg="https://www.wisetechglobal.com/"></wtg:History>
  <wtg:PackageID xmlns:wtg="https://www.wisetechglobal.com/">24</wtg:PackageID>
  <wtg:WayBillNumber xmlns:wtg="https://www.wisetechglobal.com/">WayBillNumber4</wtg:WayBillNumber>
  <wtg:ShipperReference xmlns:wtg="https://www.wisetechglobal.com/">ShipperReference6</wtg:ShipperReference>
</wtg:Package>
```

