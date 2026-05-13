
# Pierbridge Ship Response

Indicates the status of a Ship request.

## Structure

`PierbridgeShipResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TransactionIdentifier` | `String` | Optional | The unique identifier for the transaction given in the request. | String getTransactionIdentifier() | setTransactionIdentifier(String transactionIdentifier) |
| `ControlIdentifier` | `String` | Optional | The control reference for the transaction given in the request. | String getControlIdentifier() | setControlIdentifier(String controlIdentifier) |
| `CustomerVendorNumber` | `String` | Optional | A customer vendor number associated with the transaction. | String getCustomerVendorNumber() | setCustomerVendorNumber(String customerVendorNumber) |
| `Status` | [`Status`](../../doc/models/status.md) | Required | Container for transaction errors and warning elements. | Status getStatus() | setStatus(Status status) |
| `Orders` | [`Orders2`](../../doc/models/orders-2.md) | Optional | Container all orders associated with the transaction. | Orders2 getOrders() | setOrders(Orders2 orders) |
| `Carrier` | `Integer` | Optional | Numeric identifier for the carrier.<br><br>**Default**: `0` | Integer getCarrier() | setCarrier(Integer carrier) |
| `CarrierName` | `String` | Optional | The name for the carrier. | String getCarrierName() | setCarrierName(String carrierName) |
| `ServiceType` | `Integer` | Optional | Numeric identifier for the carrier service assocaited with the transaction.<br><br>**Default**: `0` | Integer getServiceType() | setServiceType(Integer serviceType) |
| `ServiceTypeName` | `String` | Optional | Description of the service used for the transaction. | String getServiceTypeName() | setServiceTypeName(String serviceTypeName) |
| `CarrierScac` | `String` | Optional | The NMFTA (National Motor Freight Traffic Association) Standard Carrier Alpha Code of the carrier. | String getCarrierScac() | setCarrierScac(String carrierScac) |
| `BrokerReference` | `String` | Optional | Broker reference. | String getBrokerReference() | setBrokerReference(String brokerReference) |
| `ConsolidatedShipmentApiIdentifier` | `String` | Optional | An identifier from an external source that identifies the consolidated shipment. | String getConsolidatedShipmentApiIdentifier() | setConsolidatedShipmentApiIdentifier(String consolidatedShipmentApiIdentifier) |
| `ExternalCarrierIdentifier` | `String` | Optional | An identifier for an external system associated with the carrier. | String getExternalCarrierIdentifier() | setExternalCarrierIdentifier(String externalCarrierIdentifier) |
| `ExternalServiceIdentifier` | `String` | Optional | An identifier for an external system associated with the carrier service. | String getExternalServiceIdentifier() | setExternalServiceIdentifier(String externalServiceIdentifier) |
| `LocationExternalSystemCode` | `String` | Optional | Code used to map the Senders location to a location in an external system. | String getLocationExternalSystemCode() | setLocationExternalSystemCode(String locationExternalSystemCode) |
| `BoLNumber` | `String` | Optional | The bill of lading number for the shipment. | String getBoLNumber() | setBoLNumber(String boLNumber) |
| `MasterBoLNumber` | `String` | Optional | The master bill of lading number for the shipment. | String getMasterBoLNumber() | setMasterBoLNumber(String masterBoLNumber) |
| `WorldEaseID` | `String` | Optional | The unique identifier for the use with UPS World Ease. | String getWorldEaseID() | setWorldEaseID(String worldEaseID) |
| `Zone` | `String` | Optional | The zone assosicated with the shipment. | String getZone() | setZone(String zone) |
| `Weight` | `Double` | Optional | Total weight of the shipment.<br><br>**Default**: `0d` | Double getWeight() | setWeight(Double weight) |
| `ServiceIsGuaranteed` | `Boolean` | Optional | Indicates if the carrier service has a guaranteed delivery window.<br><br>**Default**: `false` | Boolean getServiceIsGuaranteed() | setServiceIsGuaranteed(Boolean serviceIsGuaranteed) |
| `EDIMessageID` | `Integer` | Optional | Unique identifier for the EDI message produced during the shipment.<br><br>**Default**: `0` | Integer getEDIMessageID() | setEDIMessageID(Integer eDIMessageID) |
| `CommitmentLevel` | `String` | Optional | Returned by the carrier indicating the expected delivery date and time. | String getCommitmentLevel() | setCommitmentLevel(String commitmentLevel) |
| `VICSBoLNumber` | `String` | Optional | The VICS billing of lading number. | String getVICSBoLNumber() | setVICSBoLNumber(String vICSBoLNumber) |
| `RecordIdentifiers` | [`RecordIdentifiers3`](../../doc/models/record-identifiers-3.md) | Optional | Outer container for transaction identifiers. | RecordIdentifiers3 getRecordIdentifiers() | setRecordIdentifiers(RecordIdentifiers3 recordIdentifiers) |
| `Localization` | [`Localization1`](../../doc/models/localization-1.md) | Optional | Container for localization information. | Localization1 getLocalization() | setLocalization(Localization1 localization) |
| `Receiver` | [`Receiver5`](../../doc/models/receiver-5.md) | Optional | Container for the receiver address details associated with the transaction. | Receiver5 getReceiver() | setReceiver(Receiver5 receiver) |
| `CorrectedReceiverAddress` | [`CorrectedReceiverAddress`](../../doc/models/corrected-receiver-address.md) | Optional | Container for the receiver address returned by the carrier if address corrections have been made. | CorrectedReceiverAddress getCorrectedReceiverAddress() | setCorrectedReceiverAddress(CorrectedReceiverAddress correctedReceiverAddress) |
| `ThirdPartyHazardous` | [`ThirdPartyHazardous5`](../../doc/models/third-party-hazardous-5.md) | Optional | Container for details for processing by an external hazardous compliance system. | ThirdPartyHazardous5 getThirdPartyHazardous() | setThirdPartyHazardous(ThirdPartyHazardous5 thirdPartyHazardous) |
| `Shipping` | [`Shipping`](../../doc/models/shipping.md) | Optional | Container for shipping associated with the transaction. | Shipping getShipping() | setShipping(Shipping shipping) |
| `Customer` | [`Customer`](../../doc/models/customer.md) | Optional | Container for customer details. | Customer getCustomer() | setCustomer(Customer customer) |
| `Rates` | [`Rates8`](../../doc/models/rates-8.md) | Optional | Container all rates associated with the transaction. | Rates8 getRates() | setRates(Rates8 rates) |
| `ClientID` | `String` | Optional | Identifier for the client. | String getClientID() | setClientID(String clientID) |
| `ShipmentIdentifier` | `String` | Optional | The unique identifier assigned to the shipment. | String getShipmentIdentifier() | setShipmentIdentifier(String shipmentIdentifier) |
| `ShippingTrackingNumber` | `String` | Optional | Tracking number associated with the entire shipment. | String getShippingTrackingNumber() | setShippingTrackingNumber(String shippingTrackingNumber) |
| `EstDelivery` | `String` | Optional | The estimated date of delivery if available from the carrier. | String getEstDelivery() | setEstDelivery(String estDelivery) |
| `EstDeliveryDay` | `String` | Optional | The estimated delivery day of week if available from the carrier. | String getEstDeliveryDay() | setEstDeliveryDay(String estDeliveryDay) |
| `ShipmentID` | `Integer` | Optional | Unique identifier for the shipment.<br><br>**Default**: `0` | Integer getShipmentID() | setShipmentID(Integer shipmentID) |
| `DayOfWeek` | `String` | Optional | Day for the shipment. | String getDayOfWeek() | setDayOfWeek(String dayOfWeek) |
| `RequiredDate` | `String` | Optional | Date the items where required to be delivered by. | String getRequiredDate() | setRequiredDate(String requiredDate) |
| `SuggestedCarrier` | `Integer` | Optional | Carrier that was recommended by e.g. rate shopping.<br><br>**Default**: `0` | Integer getSuggestedCarrier() | setSuggestedCarrier(Integer suggestedCarrier) |
| `SuggestedCarrierName` | `String` | Optional | The name for the carrier. | String getSuggestedCarrierName() | setSuggestedCarrierName(String suggestedCarrierName) |
| `SuggestedServiceType` | `Integer` | Optional | Carrier service (e.g. Next Day, Ground, Express) that was recommended by e.g. rate shopping.<br><br>**Default**: `0` | Integer getSuggestedServiceType() | setSuggestedServiceType(Integer suggestedServiceType) |
| `SuggestedServiceTypeName` | `String` | Optional | Carrier service (e.g. Next Day, Ground, Express) that was recommended by e.g. rate shopping. | String getSuggestedServiceTypeName() | setSuggestedServiceTypeName(String suggestedServiceTypeName) |
| `CustomCarrierCode` | `String` | Optional | The customer's internal carrier code, if one was available that matched the carrier and service details. | String getCustomCarrierCode() | setCustomCarrierCode(String customCarrierCode) |
| `SmartPostMachinable` | `Boolean` | Optional | Indicates whether the SmartPost shipment is deemed to be machinable, based on dimensions, weight, and packaging.<br><br>**Default**: `false` | Boolean getSmartPostMachinable() | setSmartPostMachinable(Boolean smartPostMachinable) |
| `SmartPostPickupCarrier` | `String` | Optional | Identifies the carrier that will pick up the SmartPost shipment. | String getSmartPostPickupCarrier() | setSmartPostPickupCarrier(String smartPostPickupCarrier) |
| `Packages` | [`Packages8`](../../doc/models/packages-8.md) | Optional | Container for all packages associated with the transaction. | Packages8 getPackages() | setPackages(Packages8 packages) |
| `RouteCode` | `String` | Optional | The universal route or sort aid (URSA) routing code provided by the carrier. | String getRouteCode() | setRouteCode(String routeCode) |
| `Documents` | [`Documents1`](../../doc/models/documents-1.md) | Optional | Container for documents to be printed by the caller of the transaction (client). | Documents1 getDocuments() | setDocuments(Documents1 documents) |
| `AutomatedPostageAdd` | [`AutomatedPostageAdd`](../../doc/models/automated-postage-add.md) | Optional | Container for postal meter details. | AutomatedPostageAdd getAutomatedPostageAdd() | setAutomatedPostageAdd(AutomatedPostageAdd automatedPostageAdd) |
| `PersonalShipping` | [`PersonalShipping2`](../../doc/models/personal-shipping-2.md) | Optional | Container for personal shipping elements. | PersonalShipping2 getPersonalShipping() | setPersonalShipping(PersonalShipping2 personalShipping) |
| `Cartonization` | [`Cartonization3`](../../doc/models/cartonization-3.md) | Optional | Container for cartonization data for this transaction. | Cartonization3 getCartonization() | setCartonization(Cartonization3 cartonization) |
| `ServiceTypeExternalSystemCode` | `String` | Optional | Carrier and service level code for external system. | String getServiceTypeExternalSystemCode() | setServiceTypeExternalSystemCode(String serviceTypeExternalSystemCode) |
| `BillToExternalSystemCode` | `String` | Optional | Bill to code for external system. | String getBillToExternalSystemCode() | setBillToExternalSystemCode(String billToExternalSystemCode) |
| `OutputHandling` | [`OutputHandling`](../../doc/models/output-handling.md) | Optional | Container indicating handling of outputs. | OutputHandling getOutputHandling() | setOutputHandling(OutputHandling outputHandling) |
| `Processing` | [`Processing`](../../doc/models/processing.md) | Required | Container element for transaction processing statistics. | Processing getProcessing() | setProcessing(Processing processing) |

## Example (as XML)

```xml
<wtg:PierbridgeShipResponse xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Status>
  <wtg:Carrier xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Carrier>
  <wtg:ServiceType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ServiceType>
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Weight>
  <wtg:ServiceIsGuaranteed xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ServiceIsGuaranteed>
  <wtg:EDIMessageID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:EDIMessageID>
  <wtg:ShipmentID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ShipmentID>
  <wtg:SuggestedCarrier xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:SuggestedCarrier>
  <wtg:SuggestedServiceType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:SuggestedServiceType>
  <wtg:SmartPostMachinable xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SmartPostMachinable>
  <wtg:Processing xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Processing>
  <wtg:TransactionIdentifier xmlns:wtg="https://www.wisetechglobal.com/">TransactionIdentifier4</wtg:TransactionIdentifier>
  <wtg:ControlIdentifier xmlns:wtg="https://www.wisetechglobal.com/">ControlIdentifier4</wtg:ControlIdentifier>
  <wtg:CustomerVendorNumber xmlns:wtg="https://www.wisetechglobal.com/">CustomerVendorNumber6</wtg:CustomerVendorNumber>
  <wtg:Orders xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Orders>
</wtg:PierbridgeShipResponse>
```

