
# Pierbridge Void Response

Indicates the status of a Void request.

## Structure

`PierbridgeVoidResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TransactionIdentifier` | `String` | Optional | The unique identifier for the transaction given in the request. | String getTransactionIdentifier() | setTransactionIdentifier(String transactionIdentifier) |
| `ControlIdentifier` | `String` | Optional | The control reference for the transaction given in the request. | String getControlIdentifier() | setControlIdentifier(String controlIdentifier) |
| `Carrier` | `Integer` | Optional | Numeric identifier for the carrier.<br><br>**Default**: `0` | Integer getCarrier() | setCarrier(Integer carrier) |
| `CarrierName` | `String` | Optional | The name for the carrier. | String getCarrierName() | setCarrierName(String carrierName) |
| `CarrierScac` | `String` | Optional | The NMFTA (National Motor Freight Traffic Association) Standard Carrier Alpha Code of the carrier. | String getCarrierScac() | setCarrierScac(String carrierScac) |
| `PickListNumber` | `String` | Optional | The pick list number, used to identify the pick list. | String getPickListNumber() | setPickListNumber(String pickListNumber) |
| `PurchaseOrderNumber` | `String` | Optional | Purchase order number associated with the transaction. | String getPurchaseOrderNumber() | setPurchaseOrderNumber(String purchaseOrderNumber) |
| `SalesOrderNumber` | `String` | Optional | Sales order number associated with the transaction. | String getSalesOrderNumber() | setSalesOrderNumber(String salesOrderNumber) |
| `AccountNumber` | `String` | Optional | Number of the account used during the void. | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `AllPackagesVoided` | `Boolean` | Optional | Indicates if all the packages in a shipment were voided. | Boolean getAllPackagesVoided() | setAllPackagesVoided(Boolean allPackagesVoided) |
| `RecordIdentifiers` | [`RecordIdentifiers7`](../../doc/models/record-identifiers-7.md) | Optional | Outer container for transaction identifiers. | RecordIdentifiers7 getRecordIdentifiers() | setRecordIdentifiers(RecordIdentifiers7 recordIdentifiers) |
| `Packages` | [`Packages13`](../../doc/models/packages-13.md) | Optional | Container for all packages associated with the transaction. | Packages13 getPackages() | setPackages(Packages13 packages) |
| `Status` | [`Status`](../../doc/models/status.md) | Required | Container for transaction errors and warning elements. | Status getStatus() | setStatus(Status status) |
| `Processing` | [`Processing`](../../doc/models/processing.md) | Required | Container element for transaction processing statistics. | Processing getProcessing() | setProcessing(Processing processing) |

## Example (as XML)

```xml
<wtg:PierbridgeVoidResponse xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Carrier xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Carrier>
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Status>
  <wtg:Processing xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Processing>
  <wtg:TransactionIdentifier xmlns:wtg="https://www.wisetechglobal.com/">TransactionIdentifier6</wtg:TransactionIdentifier>
  <wtg:ControlIdentifier xmlns:wtg="https://www.wisetechglobal.com/">ControlIdentifier6</wtg:ControlIdentifier>
  <wtg:CarrierName xmlns:wtg="https://www.wisetechglobal.com/">CarrierName8</wtg:CarrierName>
  <wtg:CarrierScac xmlns:wtg="https://www.wisetechglobal.com/">CarrierScac6</wtg:CarrierScac>
</wtg:PierbridgeVoidResponse>
```

