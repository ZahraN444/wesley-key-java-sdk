
# Pierbridge Void Request

Cancels a shipment that had already been processing with a carrier.

## Structure

`PierbridgeVoidRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TransactionIdentifier` | `String` | Optional | A unique identifier for the transaction, this value is not used during processing and will be returned in the response. | String getTransactionIdentifier() | setTransactionIdentifier(String transactionIdentifier) |
| `ControlIdentifier` | `String` | Optional | A reference to a control which generated the request, this value is not used during processing and will be returned in the response. | String getControlIdentifier() | setControlIdentifier(String controlIdentifier) |
| `UserName` | `String` | Required | The user name to use when processing the transaction.<br><br>**Constraints**: *Minimum Length*: `1` | String getUserName() | setUserName(String userName) |
| `Live` | `Boolean` | Optional | Indicates whether the transaction is a test or live.  Defaults to system configured value if not submitted.<br><br>**Default**: `false` | Boolean getLive() | setLive(Boolean live) |
| `ShipmentID` | `Integer` | Optional | Identifier of the shipment to void.  Must submit shipment identifier, shipment group identifier, package identifier or tracking number.<br><br>**Default**: `0` | Integer getShipmentID() | setShipmentID(Integer shipmentID) |
| `DisableExecution` | `Boolean` | Optional | Indicates whether to disable the actual execution with the carrier engine for this request. Use with caution, the shipment will be recorded in the system but not executed with the carrier. Rating can be passed manually or executed with Rating Options.<br><br>**Default**: `false` | Boolean getDisableExecution() | setDisableExecution(Boolean disableExecution) |
| `ShipmentRequisitionID` | `Integer` | Optional | Identifier of the shipment requisition to void.  Must submit shipment identifier, shipment group identifier, package identifier, tracking number or shipment requisition identifier.<br><br>**Default**: `0` | Integer getShipmentRequisitionID() | setShipmentRequisitionID(Integer shipmentRequisitionID) |
| `ShipmentGroupID` | `Integer` | Optional | Identifier of the shipment group to void.  Must submit shipment identifier, shipment group identifier, package identifier or tracking number.<br><br>**Default**: `0` | Integer getShipmentGroupID() | setShipmentGroupID(Integer shipmentGroupID) |
| `AccountID` | `Integer` | Optional | Overrides the account to allow voiding using any account.<br><br>**Default**: `0` | Integer getAccountID() | setAccountID(Integer accountID) |
| `Carrier` | `Integer` | Optional | Numeric identifier for the carrier.<br><br>**Default**: `0` | Integer getCarrier() | setCarrier(Integer carrier) |
| `Packages` | [`Packages12`](../../doc/models/packages-12.md) | Optional | Container for all packages associated with the transaction. | Packages12 getPackages() | setPackages(Packages12 packages) |
| `Diagnostics` | [`Diagnostics`](../../doc/models/diagnostics.md) | Optional | Container for logging and diagnostic override elements. | Diagnostics getDiagnostics() | setDiagnostics(Diagnostics diagnostics) |
| `Identification` | [`Identification`](../../doc/models/identification.md) | Optional | Container for client identification elements. | Identification getIdentification() | setIdentification(Identification identification) |

## Example (as XML)

```xml
<wtg:PierbridgeVoidRequest xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:UserName xmlns:wtg="https://www.wisetechglobal.com/"></wtg:UserName>
  <wtg:Live xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Live>
  <wtg:ShipmentID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ShipmentID>
  <wtg:DisableExecution xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DisableExecution>
  <wtg:ShipmentRequisitionID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ShipmentRequisitionID>
  <wtg:ShipmentGroupID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ShipmentGroupID>
  <wtg:AccountID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:AccountID>
  <wtg:Carrier xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Carrier>
  <wtg:TransactionIdentifier xmlns:wtg="https://www.wisetechglobal.com/">TransactionIdentifier0</wtg:TransactionIdentifier>
  <wtg:ControlIdentifier xmlns:wtg="https://www.wisetechglobal.com/">ControlIdentifier0</wtg:ControlIdentifier>
</wtg:PierbridgeVoidRequest>
```

