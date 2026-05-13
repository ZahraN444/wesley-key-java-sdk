
# Package 9

Container for an individual package associated with the transaction.

## Structure

`Package9`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RecordIdentifiers` | [`RecordIdentifiers3`](../../doc/models/record-identifiers-3.md) | Optional | Outer container for transaction identifiers. | RecordIdentifiers3 getRecordIdentifiers() | setRecordIdentifiers(RecordIdentifiers3 recordIdentifiers) |
| `Status` | [`Status`](../../doc/models/status.md) | Required | Container for transaction errors and warning elements. | Status getStatus() | setStatus(Status status) |
| `MailPieceNumber` | `String` | Optional | Mail piece number to associate with the package. Use in association with tracking number for postal services. | String getMailPieceNumber() | setMailPieceNumber(String mailPieceNumber) |
| `UniqueIdentifier` | `String` | Optional | Free form identifier for the package. | String getUniqueIdentifier() | setUniqueIdentifier(String uniqueIdentifier) |
| `OtherIdentifier` | `String` | Optional | Free form identifier for the package. | String getOtherIdentifier() | setOtherIdentifier(String otherIdentifier) |
| `BillingCode` | `String` | Optional | Code relating to the billing. | String getBillingCode() | setBillingCode(String billingCode) |
| `SubmittedWeight` | `Double` | Optional | Indicates the weight that was submitted to the carrier in cases where weights are pre-processed by shipment server. | Double getSubmittedWeight() | setSubmittedWeight(Double submittedWeight) |
| `AdditionalHandling` | `Boolean` | Optional | Indicates that extra handling measures are required when loading the package.<br><br>**Default**: `false` | Boolean getAdditionalHandling() | setAdditionalHandling(Boolean additionalHandling) |
| `Oversize` | `Integer` | Optional | Indicates if the item is over standard size dimensions.<br><br>**Default**: `0` | Integer getOversize() | setOversize(Integer oversize) |
| `PackageType` | `Integer` | Optional | Numeric identifier for the carrier package type.<br><br>**Default**: `0` | Integer getPackageType() | setPackageType(Integer packageType) |
| `FreightClass` | `String` | Optional | The freight class of the package's content. | String getFreightClass() | setFreightClass(String freightClass) |
| `Weight` | `Double` | Optional | The weight of the package.<br><br>**Default**: `0d` | Double getWeight() | setWeight(Double weight) |
| `PackageUniqueIdentifier` | `String` | Optional | Package Unique Identifier. | String getPackageUniqueIdentifier() | setPackageUniqueIdentifier(String packageUniqueIdentifier) |
| `ShipperReference` | `String` | Optional | Primary shipping reference number. | String getShipperReference() | setShipperReference(String shipperReference) |
| `PackageReference` | `String` | Optional | Package reference number, which will be echoed back in the response. | String getPackageReference() | setPackageReference(String packageReference) |
| `FullIntelligentMailPackageBarcode` | `String` | Optional | IMpb barcode for the shipment. | String getFullIntelligentMailPackageBarcode() | setFullIntelligentMailPackageBarcode(String fullIntelligentMailPackageBarcode) |
| `WayBillNumber` | `String` | Optional | Tracking number of the package. | String getWayBillNumber() | setWayBillNumber(String wayBillNumber) |
| `WayBillNumber2` | `String` | Optional | If appropriate the secondary tracking number of the package. | String getWayBillNumber2() | setWayBillNumber2(String wayBillNumber2) |
| `OriginStation` | `String` | Optional | The carrier's station location for the origin shipper. | String getOriginStation() | setOriginStation(String originStation) |
| `RouteCode` | `String` | Optional | The universal route or sort aid (URSA) routing code provided by the carrier. | String getRouteCode() | setRouteCode(String routeCode) |
| `DestinationStation` | `String` | Optional | Contains the carrier's location identifier of the package destination, if available. | String getDestinationStation() | setDestinationStation(String destinationStation) |
| `ServiceCode` | `String` | Optional | Code for the service. | String getServiceCode() | setServiceCode(String serviceCode) |
| `BannerText` | `String` | Optional | Banner text for USPS barcodes. | String getBannerText() | setBannerText(String bannerText) |
| `FormID` | `String` | Optional | Tracking number of the package. | String getFormID() | setFormID(String formID) |
| `CODWayBillNumber` | `String` | Optional | Tracking number of the package. | String getCODWayBillNumber() | setCODWayBillNumber(String cODWayBillNumber) |
| `CODFormID` | `String` | Optional | The tracking number printed on the COD label. | String getCODFormID() | setCODFormID(String cODFormID) |
| `PackageID` | `Integer` | Optional | Unique identifier for the package. | Integer getPackageID() | setPackageID(Integer packageID) |
| `ShipToHoldState` | `Integer` | Optional | The status if the shipment has been processed using ship to hold.<br><br>**Default**: `0` | Integer getShipToHoldState() | setShipToHoldState(Integer shipToHoldState) |
| `Insurance` | [`Insurance2`](../../doc/models/insurance-2.md) | Optional | Container for insurance details. | Insurance2 getInsurance() | setInsurance(Insurance2 insurance) |
| `International` | [`International10`](../../doc/models/international-10.md) | Optional | Container for international details associated with the shipment. | International10 getInternational() | setInternational(International10 international) |
| `Labels` | [`Labels`](../../doc/models/labels.md) | Optional | Container for labels to be printed by the caller of the transaction (client). | Labels getLabels() | setLabels(Labels labels) |
| `Documents` | [`Documents`](../../doc/models/documents.md) | Optional | Container for documents to be printed by the caller of the transaction (client). | Documents getDocuments() | setDocuments(Documents documents) |
| `Shipping` | [`Shipping`](../../doc/models/shipping.md) | Optional | Container for shipping associated with the transaction. | Shipping getShipping() | setShipping(Shipping shipping) |
| `Customer` | [`Customer`](../../doc/models/customer.md) | Optional | Container for customer details. | Customer getCustomer() | setCustomer(Customer customer) |
| `Rates` | [`Rates9`](../../doc/models/rates-9.md) | Optional | Container all rates associated with the transaction. | Rates9 getRates() | setRates(Rates9 rates) |

## Example (as XML)

```xml
<wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Status>
  <wtg:AdditionalHandling xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AdditionalHandling>
  <wtg:Oversize xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Oversize>
  <wtg:PackageType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageType>
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Weight>
  <wtg:ShipToHoldState xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ShipToHoldState>
  <wtg:RecordIdentifiers xmlns:wtg="https://www.wisetechglobal.com/"></wtg:RecordIdentifiers>
  <wtg:MailPieceNumber xmlns:wtg="https://www.wisetechglobal.com/">MailPieceNumber4</wtg:MailPieceNumber>
  <wtg:UniqueIdentifier xmlns:wtg="https://www.wisetechglobal.com/">UniqueIdentifier8</wtg:UniqueIdentifier>
  <wtg:OtherIdentifier xmlns:wtg="https://www.wisetechglobal.com/">OtherIdentifier4</wtg:OtherIdentifier>
  <wtg:BillingCode xmlns:wtg="https://www.wisetechglobal.com/">BillingCode2</wtg:BillingCode>
</wtg:Package>
```

