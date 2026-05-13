
# Content 2

Container for a individual content (line item) associated with the transaction.

## Structure

`Content2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RecordIdentifiers` | [`RecordIdentifiers1`](../../doc/models/record-identifiers-1.md) | Optional | Outer container for transaction identifiers. | RecordIdentifiers1 getRecordIdentifiers() | setRecordIdentifiers(RecordIdentifiers1 recordIdentifiers) |
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
| `ContentNMFC` | `String` | Optional | Line Item National Motor Freight Classification (NMFC). | String getContentNMFC() | setContentNMFC(String contentNMFC) |
| `ContentFreightClass` | `String` | Optional | Freight Class of the line item. | String getContentFreightClass() | setContentFreightClass(String contentFreightClass) |
| `PickListID` | `Integer` | Optional | The unique numeric identifier for the pick list record.<br><br>**Default**: `0` | Integer getPickListID() | setPickListID(Integer pickListID) |
| `PackItemID` | `Integer` | Optional | Unique numeric identifier for the pack item.<br><br>**Default**: `0` | Integer getPackItemID() | setPackItemID(Integer packItemID) |
| `ContentID` | `Integer` | Optional | The unique numeric identifier for the content record.<br><br>**Default**: `0` | Integer getContentID() | setContentID(Integer contentID) |
| `PreferenceCriterion` | `String` | Optional | Preference criterion for NAFTA tariff rate. Values are A - F according to NAFTA definitions. | String getPreferenceCriterion() | setPreferenceCriterion(String preferenceCriterion) |
| `SenderIsProducer` | `Boolean` | Optional | Indicates if the sender also created the content item.<br><br>**Default**: `false` | Boolean getSenderIsProducer() | setSenderIsProducer(Boolean senderIsProducer) |
| `ProducerEvidence` | `String` | Optional | Type of evidence for the producer of the line item. Values are 1, 2 or 3 according to NAFTA definitions. | String getProducerEvidence() | setProducerEvidence(String producerEvidence) |
| `RegionalValueContentCalculatedUsingNetCostMethod` | `String` | Optional | Indicates whether the regional value content was calculated using the net cost method. | String getRegionalValueContentCalculatedUsingNetCostMethod() | setRegionalValueContentCalculatedUsingNetCostMethod(String regionalValueContentCalculatedUsingNetCostMethod) |
| `RegionalValueContentStartDate` | `String` | Optional | Date that the regional value content calculation started at. | String getRegionalValueContentStartDate() | setRegionalValueContentStartDate(String regionalValueContentStartDate) |
| `RegionalValueContentEndDate` | `String` | Optional | Date that the regional value content calculation ended. | String getRegionalValueContentEndDate() | setRegionalValueContentEndDate(String regionalValueContentEndDate) |
| `JointProduction` | `String` | Optional | Indicates whether the line item has two or more producers. | String getJointProduction() | setJointProduction(String jointProduction) |
| `PositionInContainer` | `String` | Optional | Position of the item within the shipping container. | String getPositionInContainer() | setPositionInContainer(String positionInContainer) |

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
  <wtg:PickListID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PickListID>
  <wtg:PackItemID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackItemID>
  <wtg:ContentID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ContentID>
  <wtg:SenderIsProducer xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SenderIsProducer>
  <wtg:RecordIdentifiers xmlns:wtg="https://www.wisetechglobal.com/"></wtg:RecordIdentifiers>
</wtg:Content>
```

