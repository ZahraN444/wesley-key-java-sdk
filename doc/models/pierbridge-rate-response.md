
# Pierbridge Rate Response

Contains the charges associated with the shipment given in the Rate request.

## Structure

`PierbridgeRateResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TransactionIdentifier` | `String` | Optional | The unique identifier for the transaction given in the request. | String getTransactionIdentifier() | setTransactionIdentifier(String transactionIdentifier) |
| `ControlIdentifier` | `String` | Optional | The control reference for the transaction given in the request. | String getControlIdentifier() | setControlIdentifier(String controlIdentifier) |
| `Status` | [`Status`](../../doc/models/status.md) | Required | Container for transaction errors and warning elements. | Status getStatus() | setStatus(Status status) |
| `RecordIdentifiers` | [`RecordIdentifiers`](../../doc/models/record-identifiers.md) | Optional | Outer container for transaction identifiers. | RecordIdentifiers getRecordIdentifiers() | setRecordIdentifiers(RecordIdentifiers recordIdentifiers) |
| `Carrier` | `Integer` | Optional | Numeric identifier for the carrier.<br><br>**Default**: `0` | Integer getCarrier() | setCarrier(Integer carrier) |
| `CarrierName` | `String` | Optional | The name for the carrier. | String getCarrierName() | setCarrierName(String carrierName) |
| `ServiceType` | `Integer` | Optional | Numeric identifier for the carrier service assocaited with the transaction.<br><br>**Default**: `0` | Integer getServiceType() | setServiceType(Integer serviceType) |
| `ServiceTypeName` | `String` | Optional | Description of the service used for the transaction. | String getServiceTypeName() | setServiceTypeName(String serviceTypeName) |
| `CarrierScac` | `String` | Optional | The NMFTA (National Motor Freight Traffic Association) Standard Carrier Alpha Code of the carrier. | String getCarrierScac() | setCarrierScac(String carrierScac) |
| `RateID` | `Integer` | Optional | Unique identifier for the rate.<br><br>**Default**: `0` | Integer getRateID() | setRateID(Integer rateID) |
| `DayOfWeek` | `String` | Optional | The description for the date of the shipment associated with the transaction. | String getDayOfWeek() | setDayOfWeek(String dayOfWeek) |
| `RequiredDate` | `String` | Optional | Date that the shipment is required to arrive at the receiver. | String getRequiredDate() | setRequiredDate(String requiredDate) |
| `Weight` | `Double` | Optional | Total weight of the shipment.<br><br>**Default**: `0d` | Double getWeight() | setWeight(Double weight) |
| `ServiceIsGuaranteed` | `Boolean` | Optional | Indicates if the carrier service has a guaranteed delivery window.<br><br>**Default**: `false` | Boolean getServiceIsGuaranteed() | setServiceIsGuaranteed(Boolean serviceIsGuaranteed) |
| `Localization` | [`Localization1`](../../doc/models/localization-1.md) | Optional | Container for localization information. | Localization1 getLocalization() | setLocalization(Localization1 localization) |
| `Shipping` | [`Shipping`](../../doc/models/shipping.md) | Optional | Container for shipping associated with the transaction. | Shipping getShipping() | setShipping(Shipping shipping) |
| `Customer` | [`Customer`](../../doc/models/customer.md) | Optional | Container for customer details. | Customer getCustomer() | setCustomer(Customer customer) |
| `CommitmentLevel` | `String` | Optional | Returned by the carrier indicating the expected delivery date and time. | String getCommitmentLevel() | setCommitmentLevel(String commitmentLevel) |
| `DeliverAfterTime` | `String` | Optional | Identifies a delivery window. | String getDeliverAfterTime() | setDeliverAfterTime(String deliverAfterTime) |
| `DeliveryIn` | `Integer` | Optional | Returned by the carrier indicating the number of days the shipment will take to reach its destination. | Integer getDeliveryIn() | setDeliveryIn(Integer deliveryIn) |
| `Zone` | `String` | Optional | The zone assosicated with the rate. | String getZone() | setZone(String zone) |
| `Receiver` | [`Receiver1`](../../doc/models/receiver-1.md) | Optional | Container for the receiver address details associated with the transaction. | Receiver1 getReceiver() | setReceiver(Receiver1 receiver) |
| `Rates` | [`Rates`](../../doc/models/rates.md) | Optional | Container all rates associated with the transaction. | Rates getRates() | setRates(Rates rates) |
| `Packages` | [`Packages1`](../../doc/models/packages-1.md) | Required | Container for all packages associated with the transaction. | Packages1 getPackages() | setPackages(Packages1 packages) |
| `Cartonization` | [`Cartonization1`](../../doc/models/cartonization-1.md) | Optional | Container for cartonization data for this transaction. | Cartonization1 getCartonization() | setCartonization(Cartonization1 cartonization) |
| `Processing` | [`Processing`](../../doc/models/processing.md) | Required | Container element for transaction processing statistics. | Processing getProcessing() | setProcessing(Processing processing) |

## Example (as XML)

```xml
<wtg:PierbridgeRateResponse xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Status>
  <wtg:Carrier xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Carrier>
  <wtg:ServiceType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ServiceType>
  <wtg:RateID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:RateID>
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Weight>
  <wtg:ServiceIsGuaranteed xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ServiceIsGuaranteed>
  <wtg:Packages xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:Package>
      <wtg:Status></wtg:Status>
      <wtg:AdditionalHandling>false</wtg:AdditionalHandling>
      <wtg:Oversize>0</wtg:Oversize>
      <wtg:PackageType>0</wtg:PackageType>
      <wtg:Weight>0</wtg:Weight>
      <wtg:ISOCurrencyId>0</wtg:ISOCurrencyId>
      <wtg:PackageID>0</wtg:PackageID>
      <wtg:RecordIdentifiers></wtg:RecordIdentifiers>
      <wtg:FreightClass>FreightClass6</wtg:FreightClass>
    </wtg:Package>
  </wtg:Packages>
  <wtg:Processing xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Processing>
  <wtg:TransactionIdentifier xmlns:wtg="https://www.wisetechglobal.com/">TransactionIdentifier0</wtg:TransactionIdentifier>
  <wtg:ControlIdentifier xmlns:wtg="https://www.wisetechglobal.com/">ControlIdentifier0</wtg:ControlIdentifier>
  <wtg:RecordIdentifiers xmlns:wtg="https://www.wisetechglobal.com/"></wtg:RecordIdentifiers>
  <wtg:CarrierName xmlns:wtg="https://www.wisetechglobal.com/">CarrierName6</wtg:CarrierName>
</wtg:PierbridgeRateResponse>
```

