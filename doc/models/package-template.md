
# Package Template

Container for elements to be applied to each package created from the cartonization response .

## Structure

`PackageTemplate`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Copies` | `Integer` | Optional | Indicates the number of additional copies of the package that are to be shipped.  Defaults to zero additional copies if not submitted.<br><br>**Default**: `0` | Integer getCopies() | setCopies(Integer copies) |
| `PackageRequisitionID` | `Integer` | Optional | Package Requistion of the package to ship, use this element for better multi piece requisition handling.<br><br>**Default**: `0` | Integer getPackageRequisitionID() | setPackageRequisitionID(Integer packageRequisitionID) |
| `ExternalTrackingID` | `String` | Optional | Identifier associated with Third Party Tracking. | String getExternalTrackingID() | setExternalTrackingID(String externalTrackingID) |
| `PackItemID` | `Integer` | Optional | Unique numeric identifier for the pack item.<br><br>**Default**: `0` | Integer getPackItemID() | setPackItemID(Integer packItemID) |
| `ShipperReference` | `String` | Optional | Primary reference number, which will be printed on the package's label. | String getShipperReference() | setShipperReference(String shipperReference) |
| `PackageReference` | `String` | Optional | Package reference number, which will be echoed back in the response. | String getPackageReference() | setPackageReference(String packageReference) |
| `ReceiverName` | `String` | Optional | The name of for the receiver of the package. | String getReceiverName() | setReceiverName(String receiverName) |
| `ReceiverPhone` | `String` | Optional | The phone number for the receiver of the package. | String getReceiverPhone() | setReceiverPhone(String receiverPhone) |
| `ReceiverEmail` | `String` | Optional | The email address for the receiver of the package. | String getReceiverEmail() | setReceiverEmail(String receiverEmail) |
| `SenderName` | `String` | Optional | The name for the sender of the package. | String getSenderName() | setSenderName(String senderName) |
| `SenderPhone` | `String` | Optional | The phone number for the sender of the package. | String getSenderPhone() | setSenderPhone(String senderPhone) |
| `ContentDescription` | `String` | Optional | Free form description of the package's content. | String getContentDescription() | setContentDescription(String contentDescription) |
| `WayBillNumber` | `String` | Optional | Tracking number to associate with the package. | String getWayBillNumber() | setWayBillNumber(String wayBillNumber) |
| `PriorityAlert` | `Boolean` | Optional | Indicates whether a priority alert is required for this package.  Defaults to no priority alertt if not submitted.<br><br>**Default**: `false` | Boolean getPriorityAlert() | setPriorityAlert(Boolean priorityAlert) |
| `PriorityAlertPlus` | `Boolean` | Optional | Indicates whether a priority alert plus is required for this package.  Defaults to no priority alert plus if not submitted.<br><br>**Default**: `false` | Boolean getPriorityAlertPlus() | setPriorityAlertPlus(Boolean priorityAlertPlus) |
| `Insurance` | [`Insurance`](../../doc/models/insurance.md) | Optional | Container for insurance details. | Insurance getInsurance() | setInsurance(Insurance insurance) |
| `COD` | [`COD`](../../doc/models/cod.md) | Optional | Container for collect on delivery details. | COD getCOD() | setCOD(COD cOD) |
| `GuaranteedService` | `Integer` | Optional | Numeric identifer for the type of guaranteed service.  Defaults to no guaranteed service if not submitted.<br><br>**Default**: `0` | Integer getGuaranteedService() | setGuaranteedService(Integer guaranteedService) |
| `ECOD` | `Boolean` | Optional | Electronic COD indicator. Defaults to not ECOD.<br><br>**Default**: `false` | Boolean getECOD() | setECOD(Boolean eCOD) |
| `Hold` | `Boolean` | Optional | Indicates whether the package should be held for collection at a carrier's depot or some other location.<br><br>**Default**: `false` | Boolean getHold() | setHold(Boolean hold) |
| `Holder` | [`Holder1`](../../doc/models/holder-1.md) | Optional | Container for the holding location of the package. | Holder1 getHolder() | setHolder(Holder1 holder) |
| `HomeDelivery` | [`HomeDelivery1`](../../doc/models/home-delivery-1.md) | Optional | Container for home delivery details. | HomeDelivery1 getHomeDelivery() | setHomeDelivery(HomeDelivery1 homeDelivery) |
| `HazardousPackaging` | `String` | Optional | Description of hazardous packaging. | String getHazardousPackaging() | setHazardousPackaging(String hazardousPackaging) |
| `HazardousPackageUnCode` | `String` | Optional | Description of hazardous outer packaging. | String getHazardousPackageUnCode() | setHazardousPackageUnCode(String hazardousPackageUnCode) |
| `HazardousPackagingQuantity` | `Integer` | Optional | Quantity of the outer packages.<br><br>**Default**: `0` | Integer getHazardousPackagingQuantity() | setHazardousPackagingQuantity(Integer hazardousPackagingQuantity) |
| `PackageNotes` | `String` | Optional | Package level notes. | String getPackageNotes() | setPackageNotes(String packageNotes) |
| `AdditionalHandling` | `Boolean` | Optional | Indicates that extra handling measures are required when loading the package.<br><br>**Default**: `false` | Boolean getAdditionalHandling() | setAdditionalHandling(Boolean additionalHandling) |
| `AdditionalHandlingType` | [`AdditionalHandlingTypeEnum`](../../doc/models/additional-handling-type-enum.md) | Optional | Indicates the type of Additional Handling required for this shipment. Default value is (Oversize/Overweight). | AdditionalHandlingTypeEnum getAdditionalHandlingType() | setAdditionalHandlingType(AdditionalHandlingTypeEnum additionalHandlingType) |
| `LargePackage` | `Boolean` | Optional | Indicates that package size exceeds carrier's normal limits.  Defaults to not large package if not submitted.<br><br>**Default**: `false` | Boolean getLargePackage() | setLargePackage(Boolean largePackage) |
| `DeliveryConfirmation` | `Integer` | Optional | Type of delivery confirmation required for the package.  Defaults to none if not submitted.<br><br>**Constraints**: *Pattern*: `[1-6]\|9` | Integer getDeliveryConfirmation() | setDeliveryConfirmation(Integer deliveryConfirmation) |
| `ContainerType` | `Integer` | Optional | Type of containerType required for the package.  Defaults to none if not submitted.<br><br>**Default**: `0` | Integer getContainerType() | setContainerType(Integer containerType) |
| `ExcessiveLengthType` | `Integer` | Optional | Type of excessive length required for the package.  Defaults to none if not submitted.<br><br>**Default**: `0` | Integer getExcessiveLengthType() | setExcessiveLengthType(Integer excessiveLengthType) |
| `VerbalConfirmation` | `Boolean` | Optional | Indicates verbal confirmation required. Defaults to no verbal confirmation.<br><br>**Default**: `false` | Boolean getVerbalConfirmation() | setVerbalConfirmation(Boolean verbalConfirmation) |
| `FreightClass` | `String` | Optional | The freight class of the package's content. | String getFreightClass() | setFreightClass(String freightClass) |
| `NMFC` | `String` | Optional | The National Motor Freight Classification of the package. | String getNMFC() | setNMFC(String nMFC) |
| `PalletCount` | `Integer` | Optional | Number of pallets.<br><br>**Default**: `0` | Integer getPalletCount() | setPalletCount(Integer palletCount) |
| `ItemsOnPallet` | `Integer` | Optional | Number of items on the pallet.<br><br>**Default**: `0` | Integer getItemsOnPallet() | setItemsOnPallet(Integer itemsOnPallet) |
| `NonStandardContainer` | `Boolean` | Optional | Indicates whether the package has non standard dimensions.  Defaults to standard dimensions if omitted.<br><br>**Default**: `false` | Boolean getNonStandardContainer() | setNonStandardContainer(Boolean nonStandardContainer) |
| `EmailNotification` | `Boolean` | Optional | Indicates whether an email notification should be sent to receiver's email address when package is shipped.  Defaults to not send email notification if omitted.<br><br>**Default**: `false` | Boolean getEmailNotification() | setEmailNotification(Boolean emailNotification) |
| `NonFlatMachinable` | `Boolean` | Optional | Indicates whether the package is non-flat and machinable.  Defaults to not non-flat and machinable if omitted.<br><br>**Default**: `false` | Boolean getNonFlatMachinable() | setNonFlatMachinable(Boolean nonFlatMachinable) |
| `NonMachinable` | `Boolean` | Optional | Indicates whether the package is non-machinable.  Defaults to machinable if omitted.<br><br>**Default**: `false` | Boolean getNonMachinable() | setNonMachinable(Boolean nonMachinable) |
| `NonRectangular` | `Boolean` | Optional | Indicates whether the package is non-rectangular.  Defaults to rectangular if omitted.<br><br>**Default**: `false` | Boolean getNonRectangular() | setNonRectangular(Boolean nonRectangular) |
| `Flat` | `Boolean` | Optional | Indicates whether the package is flat.  Defaults to not flat if omitted.<br><br>**Default**: `false` | Boolean getFlat() | setFlat(Boolean flat) |
| `Registered` | `Boolean` | Optional | Indicates whether the package is to be sent via registered mail.  Defaults to not registered if omitted.<br><br>**Default**: `false` | Boolean getRegistered() | setRegistered(Boolean registered) |
| `RestrictedDelivery` | `Boolean` | Optional | Indicates whether the package is to be sent using restricted delivery.  Defaults to not restricted if omitted.<br><br>**Default**: `false` | Boolean getRestrictedDelivery() | setRestrictedDelivery(Boolean restrictedDelivery) |
| `ReturnReceipt` | `Boolean` | Optional | Indicates whether a return receipt should be provided back to the shipper for this package.<br><br>**Default**: `false` | Boolean getReturnReceipt() | setReturnReceipt(Boolean returnReceipt) |
| `Certified` | `Boolean` | Optional | Indicates whether the package is to be sent via certified mail.  Defaults to not certified if omitted.<br><br>**Default**: `false` | Boolean getCertified() | setCertified(Boolean certified) |
| `DryIceWeight` | `Double` | Optional | Weight of dry ice in the package.<br><br>**Default**: `0d` | Double getDryIceWeight() | setDryIceWeight(Double dryIceWeight) |
| `DryIceWeightUOM` | `String` | Optional | Weight units of measure for the dry ice in the package. | String getDryIceWeightUOM() | setDryIceWeightUOM(String dryIceWeightUOM) |
| `ERR` | `Boolean` | Optional | Indicates that Electronic Return Receipt is required.<br><br>**Default**: `false` | Boolean getERR() | setERR(Boolean eRR) |
| `ReturnReceiptMerchandise` | `Boolean` | Optional | Indicates that Return Receipt Merchandise is required.<br><br>**Default**: `false` | Boolean getReturnReceiptMerchandise() | setReturnReceiptMerchandise(Boolean returnReceiptMerchandise) |
| `ElectronicCertified` | `Boolean` | Optional | Indicates that Electronic Certified Mail service is required.<br><br>**Default**: `false` | Boolean getElectronicCertified() | setElectronicCertified(Boolean electronicCertified) |
| `UniqueIdentifier` | `String` | Optional | Unique Identifier for a package. | String getUniqueIdentifier() | setUniqueIdentifier(String uniqueIdentifier) |
| `Exchange` | `Boolean` | Optional | Indicates whether the parcel is a consignment swap parcel. Default value is false.<br><br>**Default**: `false` | Boolean getExchange() | setExchange(Boolean exchange) |
| `AdmissibilityPackagingType` | `String` | Optional | Specific FedEx Ground non-standard container type used for domestic and cross border shipments. | String getAdmissibilityPackagingType() | setAdmissibilityPackagingType(String admissibilityPackagingType) |

## Example (as XML)

```xml
<wtg:PackageTemplate xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Copies xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Copies>
  <wtg:PackageRequisitionID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageRequisitionID>
  <wtg:PackItemID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackItemID>
  <wtg:PriorityAlert xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PriorityAlert>
  <wtg:PriorityAlertPlus xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PriorityAlertPlus>
  <wtg:GuaranteedService xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:GuaranteedService>
  <wtg:ECOD xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ECOD>
  <wtg:Hold xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Hold>
  <wtg:HazardousPackagingQuantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:HazardousPackagingQuantity>
  <wtg:AdditionalHandling xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AdditionalHandling>
  <wtg:LargePackage xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LargePackage>
  <wtg:ContainerType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ContainerType>
  <wtg:ExcessiveLengthType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ExcessiveLengthType>
  <wtg:VerbalConfirmation xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:VerbalConfirmation>
  <wtg:PalletCount xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PalletCount>
  <wtg:ItemsOnPallet xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ItemsOnPallet>
  <wtg:NonStandardContainer xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NonStandardContainer>
  <wtg:EmailNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:EmailNotification>
  <wtg:NonFlatMachinable xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NonFlatMachinable>
  <wtg:NonMachinable xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NonMachinable>
  <wtg:NonRectangular xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NonRectangular>
  <wtg:Flat xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Flat>
  <wtg:Registered xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Registered>
  <wtg:RestrictedDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:RestrictedDelivery>
  <wtg:ReturnReceipt xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReturnReceipt>
  <wtg:Certified xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Certified>
  <wtg:DryIceWeight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:DryIceWeight>
  <wtg:ERR xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ERR>
  <wtg:ReturnReceiptMerchandise xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReturnReceiptMerchandise>
  <wtg:ElectronicCertified xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ElectronicCertified>
  <wtg:Exchange xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Exchange>
  <wtg:ExternalTrackingID xmlns:wtg="https://www.wisetechglobal.com/">ExternalTrackingID6</wtg:ExternalTrackingID>
  <wtg:ShipperReference xmlns:wtg="https://www.wisetechglobal.com/">ShipperReference8</wtg:ShipperReference>
</wtg:PackageTemplate>
```

