
# Content 6

Container for a individual content (line item) associated with the transaction.

## Structure

`Content6`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RecordIdentifiers` | [`RecordIdentifiers1`](../../doc/models/record-identifiers-1.md) | Optional | Outer container for transaction identifiers. | RecordIdentifiers1 getRecordIdentifiers() | setRecordIdentifiers(RecordIdentifiers1 recordIdentifiers) |
| `Radionuclide` | [`Radionuclide`](../../doc/models/radionuclide.md) | Optional | Container for radionuclide details. | Radionuclide getRadionuclide() | setRadionuclide(Radionuclide radionuclide) |
| `Code` | `String` | Optional | Harmonized, or Schedule-B, code for the line item. | String getCode() | setCode(String code) |
| `Quantity` | `Double` | Optional | Quantity of the line item in the package.<br><br>**Default**: `0d` | Double getQuantity() | setQuantity(Double quantity) |
| `OrderedQuantity` | `Double` | Optional | Quantity of the line item that was ordered.<br><br>**Default**: `0d` | Double getOrderedQuantity() | setOrderedQuantity(Double orderedQuantity) |
| `BackOrderedQuantity` | `Double` | Optional | Quantity of the line item that is on back order.<br><br>**Default**: `0d` | Double getBackOrderedQuantity() | setBackOrderedQuantity(Double backOrderedQuantity) |
| `ContentLineValue` | `Double` | Optional | Total monetary value of the line item.<br><br>**Default**: `0d` | Double getContentLineValue() | setContentLineValue(Double contentLineValue) |
| `Value` | `Double` | Optional | Monetary value of a single line item.<br><br>**Default**: `0d` | Double getValue() | setValue(Double value) |
| `ValueCurrency` | `String` | Optional | Currency of the monetary values of the line item. | String getValueCurrency() | setValueCurrency(String valueCurrency) |
| `Weight` | `Double` | Optional | Weight of a single line item.<br><br>**Default**: `0d` | Double getWeight() | setWeight(Double weight) |
| `WeightUOM` | `String` | Optional | Weight units of the weight of a single line item. | String getWeightUOM() | setWeightUOM(String weightUOM) |
| `Description` | `String` | Optional | Description of the line item. | String getDescription() | setDescription(String description) |
| `OriginCountry` | `String` | Optional | Country of origin of the line items. | String getOriginCountry() | setOriginCountry(String originCountry) |
| `OriginRegion` | `String` | Optional | Region of origin of the line items. | String getOriginRegion() | setOriginRegion(String originRegion) |
| `PurchaseOrderNumber` | `String` | Optional | Purchase order number associated with the line items. | String getPurchaseOrderNumber() | setPurchaseOrderNumber(String purchaseOrderNumber) |
| `SalesOrderNumber` | `String` | Optional | Sales order number associated with the line items. | String getSalesOrderNumber() | setSalesOrderNumber(String salesOrderNumber) |
| `ItemCode` | `String` | Optional | Internally-used code for the line item. | String getItemCode() | setItemCode(String itemCode) |
| `ItemDescription` | `String` | Optional | Internally-used description for the line item. | String getItemDescription() | setItemDescription(String itemDescription) |
| `UnitsOfMeasure` | `String` | Optional | Units of measure for the line item. | String getUnitsOfMeasure() | setUnitsOfMeasure(String unitsOfMeasure) |
| `CustomerCode` | `String` | Optional | Customer's code for the line item. | String getCustomerCode() | setCustomerCode(String customerCode) |
| `PartNumber` | `String` | Optional | Part number for the line item. | String getPartNumber() | setPartNumber(String partNumber) |
| `BinNumber` | `String` | Optional | Bin number for the line item. | String getBinNumber() | setBinNumber(String binNumber) |
| `LotNumber` | `String` | Optional | Lot number for the line item. | String getLotNumber() | setLotNumber(String lotNumber) |
| `SerialNumber` | `String` | Optional | Serial number for the line item. | String getSerialNumber() | setSerialNumber(String serialNumber) |
| `TotalWeight` | `Double` | Optional | Total weight of the line item.<br><br>**Default**: `0d` | Double getTotalWeight() | setTotalWeight(Double totalWeight) |
| `PackagingDescription` | `String` | Optional | Description of line item's packaging. | String getPackagingDescription() | setPackagingDescription(String packagingDescription) |
| `ECCN` | `String` | Optional | The export control classification number assocaited with the content item. | String getECCN() | setECCN(String eCCN) |
| `ContentNMFC` | `String` | Optional | National Motor Freight Classification of the line item. | String getContentNMFC() | setContentNMFC(String contentNMFC) |
| `ContentFreightClass` | `String` | Optional | Freight Class of the line item. | String getContentFreightClass() | setContentFreightClass(String contentFreightClass) |
| `ProductWebPage` | `String` | Optional | The url for the the line item on the suppliers web site. | String getProductWebPage() | setProductWebPage(String productWebPage) |
| `Hazardous` | `Boolean` | Optional | Indicates whether the line item is hazardous.  Defaults to not hazardous if omitted.<br><br>**Default**: `false` | Boolean getHazardous() | setHazardous(Boolean hazardous) |
| `HazardousExemptionID` | `Integer` | Optional | Hazardous Exemption for the line item.<br><br>**Default**: `0` | Integer getHazardousExemptionID() | setHazardousExemptionID(Integer hazardousExemptionID) |
| `HazardousType` | `String` | Optional | Hazardous Type for the line item. | String getHazardousType() | setHazardousType(String hazardousType) |
| `HazardousUnits` | `Double` | Optional | Hazardous Units in each line item.<br><br>**Default**: `0d` | Double getHazardousUnits() | setHazardousUnits(Double hazardousUnits) |
| `HazardousUnitsUOM` | `String` | Optional | Hazardous units of measure for the line item. | String getHazardousUnitsUOM() | setHazardousUnitsUOM(String hazardousUnitsUOM) |
| `HazardousDescription` | `String` | Optional | Hazardous Description for the line item. | String getHazardousDescription() | setHazardousDescription(String hazardousDescription) |
| `HazardousProperShippingName` | `String` | Optional | Proper Shipping Name for the line item. | String getHazardousProperShippingName() | setHazardousProperShippingName(String hazardousProperShippingName) |
| `HazardousIdentifier` | `String` | Optional | Hazardous Material Identification Number for the line item. | String getHazardousIdentifier() | setHazardousIdentifier(String hazardousIdentifier) |
| `HazardousClass` | `String` | Optional | Hazardous Class for the line item. | String getHazardousClass() | setHazardousClass(String hazardousClass) |
| `HazardousSubClass` | `String` | Optional | Hazardous Sub-Class for the line item. | String getHazardousSubClass() | setHazardousSubClass(String hazardousSubClass) |
| `HazardousPackingGroup` | `String` | Optional | Hazardous Packing Group for the line item. | String getHazardousPackingGroup() | setHazardousPackingGroup(String hazardousPackingGroup) |
| `HazardousTechnicalName` | `String` | Optional | Hazardous Technical Name for the line item. | String getHazardousTechnicalName() | setHazardousTechnicalName(String hazardousTechnicalName) |
| `HazardousTotalQuantity` | `Double` | Optional | Total Quantity of hazardous material in this line item.<br><br>**Default**: `0d` | Double getHazardousTotalQuantity() | setHazardousTotalQuantity(Double hazardousTotalQuantity) |
| `HazardousTotalQuantityUOM` | `String` | Optional | Units of measure for total quantity of hazardous material in this line item. | String getHazardousTotalQuantityUOM() | setHazardousTotalQuantityUOM(String hazardousTotalQuantityUOM) |
| `HazardousLabelCodes` | `String` | Optional | Hazardous Label Codes for the line item. | String getHazardousLabelCodes() | setHazardousLabelCodes(String hazardousLabelCodes) |
| `HazardousLabels` | `String` | Optional | Hazardous Labels for the line item. | String getHazardousLabels() | setHazardousLabels(String hazardousLabels) |
| `HazardousAirLabels` | `String` | Optional | Hazardous Air Labels for the line item. | String getHazardousAirLabels() | setHazardousAirLabels(String hazardousAirLabels) |
| `HazardousLabelCodesMask` | `Integer` | Optional | Hazardous Label Codes Bit Mask for the line item.<br><br>**Default**: `0` | Integer getHazardousLabelCodesMask() | setHazardousLabelCodesMask(Integer hazardousLabelCodesMask) |
| `HazardousAccessible` | `Boolean` | Optional | Indicates whether the hazardous line item must remain accessible during transportation.  Defaults to not accessible if omitted.<br><br>**Default**: `false` | Boolean getHazardousAccessible() | setHazardousAccessible(Boolean hazardousAccessible) |
| `HazardousPassengerAircraft` | `Boolean` | Optional | Indicates whether the hazardous line item can be transported on a passenger aircraft.  Defaults to cannot be transported on a passenger aircraft if omitted.<br><br>**Default**: `false` | Boolean getHazardousPassengerAircraft() | setHazardousPassengerAircraft(Boolean hazardousPassengerAircraft) |
| `HazardousCargoAircraftOnly` | `Boolean` | Optional | Indicates whether the hazardous line item can only be transported on a cargo aircraft.  Defaults to not cargo aircraft only if omitted.<br><br>**Default**: `false` | Boolean getHazardousCargoAircraftOnly() | setHazardousCargoAircraftOnly(Boolean hazardousCargoAircraftOnly) |
| `HazardousRequiredInformation` | `String` | Optional | Any additional required information relating to the hazardous item, e.g. Limited Qty, permit numbers and type. | String getHazardousRequiredInformation() | setHazardousRequiredInformation(String hazardousRequiredInformation) |
| `HazardousConsumerCommodity` | `Boolean` | Optional | Indicates if an item can be classified as a consumer commodity item for the purposes of hazardous shipping.  Defaults to not consumer commodity if omitted.<br><br>**Default**: `false` | Boolean getHazardousConsumerCommodity() | setHazardousConsumerCommodity(Boolean hazardousConsumerCommodity) |
| `HazardousLimitedQuantity` | `Boolean` | Optional | Indicates if an item can be classified as a limited qunatity item for the purposes of hazardous shipping.<br><br>**Default**: `false` | Boolean getHazardousLimitedQuantity() | setHazardousLimitedQuantity(Boolean hazardousLimitedQuantity) |
| `HazardousConcentration` | `Integer` | Optional | The percentage concentration for the line item.<br><br>**Default**: `0` | Integer getHazardousConcentration() | setHazardousConcentration(Integer hazardousConcentration) |
| `Hazardous500KGExemption` | `Boolean` | Optional | Indicates if an item can be classified as meeting the 500KG exemption for the purposes of hazardous shipping.<br><br>**Default**: `false` | Boolean getHazardous500KGExemption() | setHazardous500KGExemption(Boolean hazardous500KGExemption) |
| `HazardousPackingInstructions` | `String` | Optional | Hazardous packing instructions for the product. | String getHazardousPackingInstructions() | setHazardousPackingInstructions(String hazardousPackingInstructions) |
| `HazardousIsSpecialProvisionA1A2A51A109` | `String` | Optional | Indicates if the item is to be shipped under special provisions A1, A2, A51 or A109. | String getHazardousIsSpecialProvisionA1A2A51A109() | setHazardousIsSpecialProvisionA1A2A51A109(String hazardousIsSpecialProvisionA1A2A51A109) |
| `HazardousOverpack` | `Boolean` | Optional | Flag indicates if this shipment's outer container encloses and secures one or more inner containers.<br><br>**Default**: `false` | Boolean getHazardousOverpack() | setHazardousOverpack(Boolean hazardousOverpack) |
| `HazardousAllInOne` | `Boolean` | Optional | Flag indicates if this shipment's packages are all contained in one container.<br><br>**Default**: `false` | Boolean getHazardousAllInOne() | setHazardousAllInOne(Boolean hazardousAllInOne) |
| `HazardousChemicalRecordIdentifier` | `String` | Optional | Identifies the Chemcial Record. | String getHazardousChemicalRecordIdentifier() | setHazardousChemicalRecordIdentifier(String hazardousChemicalRecordIdentifier) |
| `NumberOfInnerContainers` | `String` | Optional | The number of items packed inside the content item. | String getNumberOfInnerContainers() | setNumberOfInnerContainers(String numberOfInnerContainers) |
| `PreferenceCriterion` | `String` | Optional | Preference criterion for NAFTA tariff rate. Values are A - F according to NAFTA definitions. | String getPreferenceCriterion() | setPreferenceCriterion(String preferenceCriterion) |
| `SenderIsProducer` | `Boolean` | Optional | Indicates if the sender also created the content item.<br><br>**Default**: `false` | Boolean getSenderIsProducer() | setSenderIsProducer(Boolean senderIsProducer) |
| `JointProduction` | `Boolean` | Optional | Indicates whether the line item has two or more producers.<br><br>**Default**: `false` | Boolean getJointProduction() | setJointProduction(Boolean jointProduction) |
| `ProducerEvidence` | `Integer` | Optional | Type of evidence for the producer of the line item. Values are 1, 2 or 3 according to NAFTA definitions.<br><br>**Default**: `0` | Integer getProducerEvidence() | setProducerEvidence(Integer producerEvidence) |
| `RegionalValueContentCalculatedUsingNetCostMethod` | `Boolean` | Optional | Indicates whether the regional value content was calculated using the net cost method.<br><br>**Default**: `false` | Boolean getRegionalValueContentCalculatedUsingNetCostMethod() | setRegionalValueContentCalculatedUsingNetCostMethod(Boolean regionalValueContentCalculatedUsingNetCostMethod) |
| `RegionalValueContentStartDate` | `String` | Optional | Date that the regional value content calculation started at. | String getRegionalValueContentStartDate() | setRegionalValueContentStartDate(String regionalValueContentStartDate) |
| `RegionalValueContentEndDate` | `String` | Optional | Date that the regional value content calculation ended. | String getRegionalValueContentEndDate() | setRegionalValueContentEndDate(String regionalValueContentEndDate) |
| `NonHazardousMaterial` | `String` | Optional | String value containing the total line item weight and weight UOM. | String getNonHazardousMaterial() | setNonHazardousMaterial(String nonHazardousMaterial) |
| `HazardousClassHazardousCargoAircraftOnly` | `String` | Optional | String value containing the hazard class for cargo aircraft only shipping. | String getHazardousClassHazardousCargoAircraftOnly() | setHazardousClassHazardousCargoAircraftOnly(String hazardousClassHazardousCargoAircraftOnly) |
| `HazardousSQEIndicator` | `Boolean` | Optional | Value indicates small quantity exception in effect for this shipment.<br><br>**Default**: `false` | Boolean getHazardousSQEIndicator() | setHazardousSQEIndicator(Boolean hazardousSQEIndicator) |
| `HazardousSpecialProvision` | `String` | Optional | Value indicates the hazardous special provision in use. | String getHazardousSpecialProvision() | setHazardousSpecialProvision(String hazardousSpecialProvision) |
| `NetMassQuantity` | `Double` | Optional | Net mass quantity.<br><br>**Default**: `0d` | Double getNetMassQuantity() | setNetMassQuantity(Double netMassQuantity) |
| `NetMassUOM` | `String` | Optional | Net mass units of measure. | String getNetMassUOM() | setNetMassUOM(String netMassUOM) |
| `NetExplosive` | [`NetExplosive`](../../doc/models/net-explosive.md) | Optional | Container for net explosive details. | NetExplosive getNetExplosive() | setNetExplosive(NetExplosive netExplosive) |
| `ThirdPartyHazardous` | [`ThirdPartyHazardous4`](../../doc/models/third-party-hazardous-4.md) | Optional | Container for details for processing by an external hazardous compliance system. | ThirdPartyHazardous4 getThirdPartyHazardous() | setThirdPartyHazardous(ThirdPartyHazardous4 thirdPartyHazardous) |

## Example (as XML)

```xml
<wtg:Content xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Quantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Quantity>
  <wtg:OrderedQuantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:OrderedQuantity>
  <wtg:BackOrderedQuantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:BackOrderedQuantity>
  <wtg:ContentLineValue xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ContentLineValue>
  <wtg:Value xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Value>
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Weight>
  <wtg:TotalWeight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TotalWeight>
  <wtg:Hazardous xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Hazardous>
  <wtg:HazardousExemptionID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:HazardousExemptionID>
  <wtg:HazardousUnits xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:HazardousUnits>
  <wtg:HazardousTotalQuantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:HazardousTotalQuantity>
  <wtg:HazardousLabelCodesMask xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:HazardousLabelCodesMask>
  <wtg:HazardousAccessible xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HazardousAccessible>
  <wtg:HazardousPassengerAircraft xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HazardousPassengerAircraft>
  <wtg:HazardousCargoAircraftOnly xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HazardousCargoAircraftOnly>
  <wtg:HazardousConsumerCommodity xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HazardousConsumerCommodity>
  <wtg:HazardousLimitedQuantity xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HazardousLimitedQuantity>
  <wtg:HazardousConcentration xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:HazardousConcentration>
  <wtg:Hazardous500KGExemption xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Hazardous500KGExemption>
  <wtg:HazardousOverpack xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HazardousOverpack>
  <wtg:HazardousAllInOne xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HazardousAllInOne>
  <wtg:SenderIsProducer xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SenderIsProducer>
  <wtg:JointProduction xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:JointProduction>
  <wtg:ProducerEvidence xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ProducerEvidence>
  <wtg:RegionalValueContentCalculatedUsingNetCostMethod xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:RegionalValueContentCalculatedUsingNetCostMethod>
  <wtg:HazardousSQEIndicator xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HazardousSQEIndicator>
  <wtg:NetMassQuantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:NetMassQuantity>
  <wtg:RecordIdentifiers xmlns:wtg="https://www.wisetechglobal.com/"></wtg:RecordIdentifiers>
  <wtg:Radionuclide xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Radionuclide>
  <wtg:Code xmlns:wtg="https://www.wisetechglobal.com/">Code6</wtg:Code>
</wtg:Content>
```

