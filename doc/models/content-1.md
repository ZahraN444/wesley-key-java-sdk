
# Content 1

Container for an individual content associated with the transaction.

## Structure

`Content1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ContentRefNumber` | `String` | Optional | Unique reference number for the content. | String getContentRefNumber() | setContentRefNumber(String contentRefNumber) |
| `Height` | `Double` | Optional | Height of the content. | Double getHeight() | setHeight(Double height) |
| `Width` | `Double` | Optional | Width of the content. | Double getWidth() | setWidth(Double width) |
| `Length` | `Double` | Optional | Length of the content. | Double getLength() | setLength(Double length) |
| `Code` | `String` | Optional | Harmonized, or Schedule-B, code for the line item. | String getCode() | setCode(String code) |
| `Quantity` | `Integer` | Optional | Quantity of the content. | Integer getQuantity() | setQuantity(Integer quantity) |
| `UnitValue` | `Double` | Optional | Unit value of the content. | Double getUnitValue() | setUnitValue(Double unitValue) |
| `UnitWeight` | `Double` | Optional | Unit Weight of the content. | Double getUnitWeight() | setUnitWeight(Double unitWeight) |
| `Description` | `String` | Optional | Name of the content. | String getDescription() | setDescription(String description) |
| `OriginCountry` | `String` | Optional | Country of origin of the line items. | String getOriginCountry() | setOriginCountry(String originCountry) |
| `ItemCode` | `String` | Optional | Internally-used code for the line item. | String getItemCode() | setItemCode(String itemCode) |
| `ItemDescription` | `String` | Optional | Internally-used description for the line item. | String getItemDescription() | setItemDescription(String itemDescription) |
| `UnitsOfMeasure` | `String` | Optional | Units of measure for the line item. | String getUnitsOfMeasure() | setUnitsOfMeasure(String unitsOfMeasure) |
| `PartNumber` | `String` | Optional | Part number for the line item. | String getPartNumber() | setPartNumber(String partNumber) |
| `BinNumber` | `String` | Optional | Bin number for the line item. | String getBinNumber() | setBinNumber(String binNumber) |
| `LotNumber` | `String` | Optional | Lot number for the line item. | String getLotNumber() | setLotNumber(String lotNumber) |
| `Virtual` | `Boolean` | Optional | Whether or not this is a real item or a virtual, blocking space (from a subspace or loading rules) | Boolean getVirtual() | setVirtual(Boolean virtual) |
| `Sequence` | `String` | Optional | A sequence value for the item. This is intended for aisle-bin locations, e.g., aisle 11 bin 20 can be '1120’. See api.paccurate.io/docs | String getSequence() | setSequence(String sequence) |
| `CenterOfMass` | [`Point`](../../doc/models/point.md) | Optional | Center of mass | Point getCenterOfMass() | setCenterOfMass(Point centerOfMass) |

## Example (as XML)

```xml
<wtg:Content xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ContentRefNumber xmlns:wtg="https://www.wisetechglobal.com/">ContentRefNumber6</wtg:ContentRefNumber>
  <wtg:Height xmlns:wtg="https://www.wisetechglobal.com/">102.88</wtg:Height>
  <wtg:Width xmlns:wtg="https://www.wisetechglobal.com/">101.52</wtg:Width>
  <wtg:Length xmlns:wtg="https://www.wisetechglobal.com/">152.08</wtg:Length>
  <wtg:Code xmlns:wtg="https://www.wisetechglobal.com/">Code2</wtg:Code>
</wtg:Content>
```

