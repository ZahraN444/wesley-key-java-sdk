
# Package 7

Container for an individual package associated with the transaction.

## Structure

`Package7`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RecordIdentifiers` | [`RecordIdentifiers`](../../doc/models/record-identifiers.md) | Optional | Outer container for transaction identifiers. | RecordIdentifiers getRecordIdentifiers() | setRecordIdentifiers(RecordIdentifiers recordIdentifiers) |
| `ProactiveResponse` | `Boolean` | Optional | Indicates whether the package requires the Proactive Response special service.<br><br>**Default**: `false` | Boolean getProactiveResponse() | setProactiveResponse(Boolean proactiveResponse) |
| `SpecialCare` | [`SpecialCare`](../../doc/models/special-care.md) | Optional | Outer container for special care details for package. | SpecialCare getSpecialCare() | setSpecialCare(SpecialCare specialCare) |
| `LithiumBattery` | `Boolean` | Optional | Indicates whether the shipment contains a lithium battery.  Defaults to no.<br><br>**Default**: `false` | Boolean getLithiumBattery() | setLithiumBattery(Boolean lithiumBattery) |
| `LithiumBatteryDetails` | [`LithiumBatteryDetails`](../../doc/models/lithium-battery-details.md) | Optional | Outer container for Lithium Battery details for package. | LithiumBatteryDetails getLithiumBatteryDetails() | setLithiumBatteryDetails(LithiumBatteryDetails lithiumBatteryDetails) |
| `Copies` | `Integer` | Optional | Indicates the number of additional copies of the package that are to be shipped.  Defaults to zero additional copies if not submitted.<br><br>**Default**: `0` | Integer getCopies() | setCopies(Integer copies) |
| `PackageRequisitionID` | `Integer` | Optional | Package Requistion of the package to ship, use this element for better multi piece requisition handling.<br><br>**Default**: `0` | Integer getPackageRequisitionID() | setPackageRequisitionID(Integer packageRequisitionID) |
| `ExternalTrackingID` | `String` | Optional | Identifier associated with Third Party Tracking. | String getExternalTrackingID() | setExternalTrackingID(String externalTrackingID) |
| `PackItemID` | `Integer` | Optional | Unique numeric identifier for the pack item.<br><br>**Default**: `0` | Integer getPackItemID() | setPackItemID(Integer packItemID) |
| `PackageID` | `Integer` | Optional | Deprecated.  Do not use.<br><br>**Default**: `0` | Integer getPackageID() | setPackageID(Integer packageID) |
| `ShipperReference` | `String` | Optional | Primary reference number, which will be printed on the package's label. | String getShipperReference() | setShipperReference(String shipperReference) |
| `PackageReference` | `String` | Optional | Package reference number, which will be echoed back in the response. | String getPackageReference() | setPackageReference(String packageReference) |
| `ReferenceOne` | `String` | Optional | First additional reference number. | String getReferenceOne() | setReferenceOne(String referenceOne) |
| `ReferenceTwo` | `String` | Optional | Second additional reference number. | String getReferenceTwo() | setReferenceTwo(String referenceTwo) |
| `ReferenceThree` | `String` | Optional | Third additional reference number. | String getReferenceThree() | setReferenceThree(String referenceThree) |
| `ReferenceFour` | `String` | Optional | Fourth additional reference number. | String getReferenceFour() | setReferenceFour(String referenceFour) |
| `ReferenceFive` | `String` | Optional | Fifth additional reference number. | String getReferenceFive() | setReferenceFive(String referenceFive) |
| `ReferenceSix` | `String` | Optional | Sixth additional reference number. | String getReferenceSix() | setReferenceSix(String referenceSix) |
| `ReceiverName` | `String` | Optional | The name of for the receiver of the package. | String getReceiverName() | setReceiverName(String receiverName) |
| `ReceiverPhone` | `String` | Optional | The phone number for the receiver of the package. | String getReceiverPhone() | setReceiverPhone(String receiverPhone) |
| `ReceiverSecondaryPhone` | `String` | Optional | The secondary phone number for the receiver of the package. | String getReceiverSecondaryPhone() | setReceiverSecondaryPhone(String receiverSecondaryPhone) |
| `ReceiverEmail` | `String` | Optional | The email address for the receiver of the package. | String getReceiverEmail() | setReceiverEmail(String receiverEmail) |
| `SenderName` | `String` | Optional | The name for the sender of the package. | String getSenderName() | setSenderName(String senderName) |
| `SenderPhone` | `String` | Optional | The phone number for the sender of the package. | String getSenderPhone() | setSenderPhone(String senderPhone) |
| `PackageType` | `Integer` | Optional | Carrier package (e.g. letter, package, pallet) that is to be shipped.<br><br>**Default**: `0` | Integer getPackageType() | setPackageType(Integer packageType) |
| `Weight` | `Double` | Optional | The weight of the package.<br><br>**Default**: `0d` | Double getWeight() | setWeight(Double weight) |
| `MajorWeight` | `Double` | Optional | Major Weight of the package.<br><br>**Default**: `0d` | Double getMajorWeight() | setMajorWeight(Double majorWeight) |
| `MinorWeight` | `Double` | Optional | Minor Weight of the package.<br><br>**Default**: `0d` | Double getMinorWeight() | setMinorWeight(Double minorWeight) |
| `WeightUOM` | `String` | Optional | The units of measure for the package weight. | String getWeightUOM() | setWeightUOM(String weightUOM) |
| `Length` | `Double` | Optional | The dimensional lenth of the package.<br><br>**Default**: `0d` | Double getLength() | setLength(Double length) |
| `Width` | `Double` | Optional | The dimensional width of the package.<br><br>**Default**: `0d` | Double getWidth() | setWidth(Double width) |
| `Height` | `Double` | Optional | The dimensional height of the package.<br><br>**Default**: `0d` | Double getHeight() | setHeight(Double height) |
| `Cubic` | `Double` | Optional | Cubic feet or metres of the package.<br><br>**Default**: `0d` | Double getCubic() | setCubic(Double cubic) |
| `Linear` | `Double` | Optional | Linear feet or metres of the package.<br><br>**Default**: `0d` | Double getLinear() | setLinear(Double linear) |
| `DimensionsUOM` | `String` | Optional | The units of measure for the package length, width and height. | String getDimensionsUOM() | setDimensionsUOM(String dimensionsUOM) |
| `ContentDescription` | `String` | Optional | Free form description of the package's content. | String getContentDescription() | setContentDescription(String contentDescription) |
| `WayBillNumber` | `String` | Optional | Tracking number to associate with the package. | String getWayBillNumber() | setWayBillNumber(String wayBillNumber) |
| `WayBillNumber2` | `String` | Optional | If appropriate the secondary tracking number of the package. | String getWayBillNumber2() | setWayBillNumber2(String wayBillNumber2) |
| `SecurityWayBillNumber` | `String` | Optional | Tracking number to associate with the package for chain of signature services. | String getSecurityWayBillNumber() | setSecurityWayBillNumber(String securityWayBillNumber) |
| `MailPieceNumber` | `String` | Optional | Mail piece number to associate with the package. Use in association with tracking number for postal services. | String getMailPieceNumber() | setMailPieceNumber(String mailPieceNumber) |
| `PriorityAlert` | `Boolean` | Optional | Indicates whether a priority alert is required for this package.  Defaults to no priority alert if not submitted.<br><br>**Default**: `false` | Boolean getPriorityAlert() | setPriorityAlert(Boolean priorityAlert) |
| `PriorityAlertPlus` | `Boolean` | Optional | Indicates whether a priority alert plus is required for this package.  Defaults to no priority alert plus if not submitted.<br><br>**Default**: `false` | Boolean getPriorityAlertPlus() | setPriorityAlertPlus(Boolean priorityAlertPlus) |
| `ThirdPartyConsignee` | `Boolean` | Optional | Indicates selection of Third Party Consignee Special Service.<br><br>**Default**: `false` | Boolean getThirdPartyConsignee() | setThirdPartyConsignee(Boolean thirdPartyConsignee) |
| `PriorityAlertContent` | `String` | Optional | Specifies any associated details for priority alert for this package.  Defaults to none. | String getPriorityAlertContent() | setPriorityAlertContent(String priorityAlertContent) |
| `InsideDelivery` | `Boolean` | Optional | Indicates use of FedEx service: Inside Delivery.<br><br>**Default**: `false` | Boolean getInsideDelivery() | setInsideDelivery(Boolean insideDelivery) |
| `Insurance` | [`Insurance`](../../doc/models/insurance.md) | Optional | Container for insurance details. | Insurance getInsurance() | setInsurance(Insurance insurance) |
| `COD` | [`COD`](../../doc/models/cod.md) | Optional | Container for collect on delivery details. | COD getCOD() | setCOD(COD cOD) |
| `GuaranteedService` | `Integer` | Optional | Numeric identifer for the type of guaranteed service.  Defaults to no guaranteed service if not submitted.<br><br>**Default**: `0` | Integer getGuaranteedService() | setGuaranteedService(Integer guaranteedService) |
| `ECOD` | `Boolean` | Optional | Electronic COD indicator. Defaults to not ECOD.<br><br>**Default**: `false` | Boolean getECOD() | setECOD(Boolean eCOD) |
| `HoldDeliveryType` | [`HoldDeliveryTypeEnum`](../../doc/models/hold-delivery-type-enum.md) | Optional | Numeric identifer for the type of cash on delivery.  Defaults to no cash on delivery if not submitted.<br><br>**Default**: `HoldDeliveryTypeEnum.DELIVERDIRECTTOHOLDLOCATION` | HoldDeliveryTypeEnum getHoldDeliveryType() | setHoldDeliveryType(HoldDeliveryTypeEnum holdDeliveryType) |
| `Hold` | `Boolean` | Optional | Indicates whether the package should be held for collection at a carrier's depot or some other location.<br><br>**Default**: `false` | Boolean getHold() | setHold(Boolean hold) |
| `Holder` | [`Holder`](../../doc/models/holder.md) | Optional | Container for the holding location of the package. | Holder getHolder() | setHolder(Holder holder) |
| `HazardousPackaging` | `String` | Optional | Description of hazardous packaging. | String getHazardousPackaging() | setHazardousPackaging(String hazardousPackaging) |
| `HazardousPackageUnCode` | `String` | Optional | UN Code of hazardous packaging. | String getHazardousPackageUnCode() | setHazardousPackageUnCode(String hazardousPackageUnCode) |
| `HazardousPackagingQuantity` | `Integer` | Optional | Quantity of the outer packages.<br><br>**Default**: `0` | Integer getHazardousPackagingQuantity() | setHazardousPackagingQuantity(Integer hazardousPackagingQuantity) |
| `PackageNotes` | `String` | Optional | Package level notes. | String getPackageNotes() | setPackageNotes(String packageNotes) |
| `AdditionalHandling` | `Boolean` | Optional | Indicates that extra handling measures are required when loading the package.<br><br>**Default**: `false` | Boolean getAdditionalHandling() | setAdditionalHandling(Boolean additionalHandling) |
| `AdditionalHandlingType` | [`AdditionalHandlingTypeEnum`](../../doc/models/additional-handling-type-enum.md) | Optional | Indicates the type of Additional Handling required for this shipment. Default value is (Oversize/Overweight). | AdditionalHandlingTypeEnum getAdditionalHandlingType() | setAdditionalHandlingType(AdditionalHandlingTypeEnum additionalHandlingType) |
| `LargePackage` | `Boolean` | Optional | Indicates that package size exceeds carrier's normal limits.  Defaults to not large package if not submitted.<br><br>**Default**: `false` | Boolean getLargePackage() | setLargePackage(Boolean largePackage) |
| `DeliveryConfirmation` | `Integer` | Optional | Type of delivery confirmation required for the package.  Defaults to none if not submitted.<br><br>**Default**: `0` | Integer getDeliveryConfirmation() | setDeliveryConfirmation(Integer deliveryConfirmation) |
| `ContainerType` | `Integer` | Optional | Type of containerType required for the package.  Defaults to none if not submitted.<br><br>**Default**: `0` | Integer getContainerType() | setContainerType(Integer containerType) |
| `ExcessiveLengthType` | `Integer` | Optional | Type of excessive length required for the package.  Defaults to none if not submitted.<br><br>**Default**: `0` | Integer getExcessiveLengthType() | setExcessiveLengthType(Integer excessiveLengthType) |
| `VerbalConfirmation` | `Boolean` | Optional | Indicates verbal confirmation required. Defaults to no verbal confirmation.<br><br>**Default**: `false` | Boolean getVerbalConfirmation() | setVerbalConfirmation(Boolean verbalConfirmation) |
| `VerbalConfirmationContactName` | `String` | Optional | Person to pass verbal confirmation to. | String getVerbalConfirmationContactName() | setVerbalConfirmationContactName(String verbalConfirmationContactName) |
| `VerbalConfirmationPhone` | `String` | Optional | Phone number for verbal confirmation. | String getVerbalConfirmationPhone() | setVerbalConfirmationPhone(String verbalConfirmationPhone) |
| `FreightClass` | `String` | Optional | The freight class of the package's content. | String getFreightClass() | setFreightClass(String freightClass) |
| `NMFC` | `String` | Optional | The National Motor Freight Classification of the package. | String getNMFC() | setNMFC(String nMFC) |
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
| `RefrigerationRequired` | `Boolean` | Optional | Indicates whether refrigeration is required for the package<br><br>**Default**: `false` | Boolean getRefrigerationRequired() | setRefrigerationRequired(Boolean refrigerationRequired) |
| `LooseDryIce` | `Boolean` | Optional | Indicates overpacked or all-in-one hazardous package has loose dry ice<br><br>**Default**: `false` | Boolean getLooseDryIce() | setLooseDryIce(Boolean looseDryIce) |
| `ERR` | `Boolean` | Optional | Indicates that Electronic Return Receipt is required.<br><br>**Default**: `false` | Boolean getERR() | setERR(Boolean eRR) |
| `ReturnReceiptMerchandise` | `Boolean` | Optional | Indicates that Return Receipt Merchandise is required.<br><br>**Default**: `false` | Boolean getReturnReceiptMerchandise() | setReturnReceiptMerchandise(Boolean returnReceiptMerchandise) |
| `ElectronicCertified` | `Boolean` | Optional | Indicates that Electronic Certified Mail service is required.<br><br>**Default**: `false` | Boolean getElectronicCertified() | setElectronicCertified(Boolean electronicCertified) |
| `UniqueIdentifier` | `String` | Optional | Unique Identifier for a package. | String getUniqueIdentifier() | setUniqueIdentifier(String uniqueIdentifier) |
| `Exchange` | `Boolean` | Optional | Indicates whether the parcel is a consignment swap parcel. Default value is false.<br><br>**Default**: `false` | Boolean getExchange() | setExchange(Boolean exchange) |
| `AdmissibilityPackagingType` | `String` | Optional | Specific FedEx Ground non-standard container type used for domestic and cross border shipments. | String getAdmissibilityPackagingType() | setAdmissibilityPackagingType(String admissibilityPackagingType) |
| `HazardousQValue` | `String` | Optional | This represents the Q Value calculated in accordance with IATA Regulations. Values are 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0 | String getHazardousQValue() | setHazardousQValue(String hazardousQValue) |
| `International` | [`International9`](../../doc/models/international-9.md) | Optional | Container for international details associated with the shipment. | International9 getInternational() | setInternational(International9 international) |
| `Rates` | [`Rates4`](../../doc/models/rates-4.md) | Optional | Container all rates associated with the transaction. | Rates4 getRates() | setRates(Rates4 rates) |

## Example (as XML)

```xml
<wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ProactiveResponse xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ProactiveResponse>
  <wtg:LithiumBattery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LithiumBattery>
  <wtg:Copies xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Copies>
  <wtg:PackageRequisitionID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageRequisitionID>
  <wtg:PackItemID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackItemID>
  <wtg:PackageID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageID>
  <wtg:PackageType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageType>
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Weight>
  <wtg:MajorWeight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:MajorWeight>
  <wtg:MinorWeight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:MinorWeight>
  <wtg:Length xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Length>
  <wtg:Width xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Width>
  <wtg:Height xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Height>
  <wtg:Cubic xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Cubic>
  <wtg:Linear xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Linear>
  <wtg:PriorityAlert xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PriorityAlert>
  <wtg:PriorityAlertPlus xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PriorityAlertPlus>
  <wtg:ThirdPartyConsignee xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ThirdPartyConsignee>
  <wtg:InsideDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:InsideDelivery>
  <wtg:GuaranteedService xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:GuaranteedService>
  <wtg:ECOD xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ECOD>
  <wtg:HoldDeliveryType xmlns:wtg="https://www.wisetechglobal.com/">DeliverDirectToHoldLocation</wtg:HoldDeliveryType>
  <wtg:Hold xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Hold>
  <wtg:HazardousPackagingQuantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:HazardousPackagingQuantity>
  <wtg:AdditionalHandling xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AdditionalHandling>
  <wtg:LargePackage xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LargePackage>
  <wtg:DeliveryConfirmation xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:DeliveryConfirmation>
  <wtg:ContainerType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ContainerType>
  <wtg:ExcessiveLengthType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ExcessiveLengthType>
  <wtg:VerbalConfirmation xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:VerbalConfirmation>
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
  <wtg:RefrigerationRequired xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:RefrigerationRequired>
  <wtg:LooseDryIce xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LooseDryIce>
  <wtg:ERR xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ERR>
  <wtg:ReturnReceiptMerchandise xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReturnReceiptMerchandise>
  <wtg:ElectronicCertified xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ElectronicCertified>
  <wtg:Exchange xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Exchange>
  <wtg:RecordIdentifiers xmlns:wtg="https://www.wisetechglobal.com/"></wtg:RecordIdentifiers>
  <wtg:SpecialCare xmlns:wtg="https://www.wisetechglobal.com/"></wtg:SpecialCare>
  <wtg:LithiumBatteryDetails xmlns:wtg="https://www.wisetechglobal.com/"></wtg:LithiumBatteryDetails>
</wtg:Package>
```

