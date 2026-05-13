
# Content 5

Container for a individual content (line item) associated with the transaction.

## Structure

`Content5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ContentCode` | `String` | Optional | Harmonized, or Schedule-B, code for the item. | String getContentCode() | setContentCode(String contentCode) |
| `Code` | `String` | Optional | Harmonized, or Schedule-B, code for the line item. | String getCode() | setCode(String code) |
| `Quantity` | `double` | Required | Quantity of the line item in the package.<br><br>**Default**: `0d` | double getQuantity() | setQuantity(double quantity) |
| `OrderedQuantity` | `Double` | Optional | Quantity of the line item that was ordered.<br><br>**Default**: `0d` | Double getOrderedQuantity() | setOrderedQuantity(Double orderedQuantity) |
| `BackOrderedQuantity` | `Double` | Optional | Quantity of the line item that is on back order.<br><br>**Default**: `0d` | Double getBackOrderedQuantity() | setBackOrderedQuantity(Double backOrderedQuantity) |
| `ContentLineValue` | `Double` | Optional | Total monetary value of the line item.<br><br>**Default**: `0d` | Double getContentLineValue() | setContentLineValue(Double contentLineValue) |
| `Value` | `double` | Required | Monetary value of a single line item.<br><br>**Default**: `0d` | double getValue() | setValue(double value) |
| `ValueCurrency` | `String` | Optional | Currency of the monetary values of the line item. | String getValueCurrency() | setValueCurrency(String valueCurrency) |
| `Weight` | `double` | Required | Weight of a single line item.<br><br>**Default**: `0d` | double getWeight() | setWeight(double weight) |
| `WeightUOM` | `String` | Optional | Weight units of the weight of a single line item. | String getWeightUOM() | setWeightUOM(String weightUOM) |
| `Description` | `String` | Optional | Description of the line item. | String getDescription() | setDescription(String description) |
| `OriginCountry` | `String` | Required | Country of origin of the line items. | String getOriginCountry() | setOriginCountry(String originCountry) |
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
| `ContentNMFC` | `String` | Optional | National Motor Freight Classification of the line item. | String getContentNMFC() | setContentNMFC(String contentNMFC) |
| `ContentFreightClass` | `String` | Optional | Freight Class of the line item. | String getContentFreightClass() | setContentFreightClass(String contentFreightClass) |

## Example (as XML)

```xml
<wtg:Content xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Quantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Quantity>
  <wtg:OrderedQuantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:OrderedQuantity>
  <wtg:BackOrderedQuantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:BackOrderedQuantity>
  <wtg:ContentLineValue xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ContentLineValue>
  <wtg:Value xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Value>
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Weight>
  <wtg:OriginCountry xmlns:wtg="https://www.wisetechglobal.com/"></wtg:OriginCountry>
  <wtg:TotalWeight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TotalWeight>
  <wtg:ContentCode xmlns:wtg="https://www.wisetechglobal.com/">ContentCode4</wtg:ContentCode>
  <wtg:Code xmlns:wtg="https://www.wisetechglobal.com/">Code2</wtg:Code>
</wtg:Content>
```

