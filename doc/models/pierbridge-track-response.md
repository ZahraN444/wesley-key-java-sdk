
# Pierbridge Track Response

Contains details about the latest status of a shipment as defined by a Track request.

## Structure

`PierbridgeTrackResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TransactionIdentifier` | `String` | Optional | The unique identifier for the transaction given in the request. | String getTransactionIdentifier() | setTransactionIdentifier(String transactionIdentifier) |
| `ControlIdentifier` | `String` | Optional | The control reference for the transaction given in the request. | String getControlIdentifier() | setControlIdentifier(String controlIdentifier) |
| `ShipDate` | `String` | Optional | Date the items where shipped. | String getShipDate() | setShipDate(String shipDate) |
| `Service` | `String` | Optional | The carrier service description. | String getService() | setService(String service) |
| `Carrier` | `Integer` | Optional | Numeric identifier for the carrier.<br><br>**Default**: `0` | Integer getCarrier() | setCarrier(Integer carrier) |
| `CarrierName` | `String` | Optional | The name for the carrier. | String getCarrierName() | setCarrierName(String carrierName) |
| `ServiceType` | `Integer` | Optional | Numeric identifier for the carrier service associated with the transaction.<br><br>**Default**: `0` | Integer getServiceType() | setServiceType(Integer serviceType) |
| `ServiceTypeName` | `String` | Optional | Description of the service used for the transaction. | String getServiceTypeName() | setServiceTypeName(String serviceTypeName) |
| `CarrierScac` | `String` | Optional | The NMFTA (National Motor Freight Traffic Association) Standard Carrier Alpha Code of the carrier. | String getCarrierScac() | setCarrierScac(String carrierScac) |
| `Sender` | [`Sender4`](../../doc/models/sender-4.md) | Optional | Container to allow the customization of the sender address details associated with the transaction. | Sender4 getSender() | setSender(Sender4 sender) |
| `Receiver` | [`Receiver6`](../../doc/models/receiver-6.md) | Optional | Container for the receiver address details associated with the transaction. | Receiver6 getReceiver() | setReceiver(Receiver6 receiver) |
| `Packages` | [`Packages11`](../../doc/models/packages-11.md) | Optional | Container for all packages associated with the transaction. | Packages11 getPackages() | setPackages(Packages11 packages) |
| `Status` | [`Status`](../../doc/models/status.md) | Required | Container for transaction errors and warning elements. | Status getStatus() | setStatus(Status status) |
| `Processing` | [`Processing`](../../doc/models/processing.md) | Required | Container element for transaction processing statistics. | Processing getProcessing() | setProcessing(Processing processing) |

## Example (as XML)

```xml
<wtg:PierbridgeTrackResponse xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Carrier xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Carrier>
  <wtg:ServiceType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ServiceType>
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Status>
  <wtg:Processing xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Processing>
  <wtg:TransactionIdentifier xmlns:wtg="https://www.wisetechglobal.com/">TransactionIdentifier8</wtg:TransactionIdentifier>
  <wtg:ControlIdentifier xmlns:wtg="https://www.wisetechglobal.com/">ControlIdentifier8</wtg:ControlIdentifier>
  <wtg:ShipDate xmlns:wtg="https://www.wisetechglobal.com/">ShipDate4</wtg:ShipDate>
  <wtg:Service xmlns:wtg="https://www.wisetechglobal.com/">Service8</wtg:Service>
</wtg:PierbridgeTrackResponse>
```

