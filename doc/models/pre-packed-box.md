
# Pre Packed Box

## Structure

`PrePackedBox`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Name` | `String` | Optional | name for the type of box. | String getName() | setName(String name) |
| `WeightTare` | `Double` | Optional | weight of the container when empty or otherwise unladen, i.e., of the box itself. | Double getWeightTare() | setWeightTare(Double weightTare) |
| `WeightMax` | `Double` | Optional | maximum allowable gross weight for the box, i.e., all packed item weights plus the WeightTare. | Double getWeightMax() | setWeightMax(Double weightMax) |
| `Height` | `Double` | Optional | Height of the box. | Double getHeight() | setHeight(Double height) |
| `Width` | `Double` | Optional | Width of the box. | Double getWidth() | setWidth(Double width) |
| `Length` | `Double` | Optional | Length of the box. | Double getLength() | setLength(Double length) |
| `CenterOfMass` | [`Point`](../../doc/models/point.md) | Optional | 3-dimensional Coordinates of the box's center of mass | Point getCenterOfMass() | setCenterOfMass(Point centerOfMass) |
| `ID` | `Integer` | Optional | box ID<br><br>**Default**: `0` | Integer getID() | setID(Integer iD) |
| `Items` | [`Items`](../../doc/models/items.md) | Optional | Items already packed into box | Items getItems() | setItems(Items items) |
| `BoxType` | [`BoxType`](../../doc/models/box-type.md) | Required | box type | BoxType getBoxType() | setBoxType(BoxType boxType) |

## Example (as XML)

```xml
<wtg:PrePackedBox xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ID>
  <wtg:BoxType xmlns:wtg="https://www.wisetechglobal.com/"></wtg:BoxType>
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name2</wtg:Name>
  <wtg:WeightTare xmlns:wtg="https://www.wisetechglobal.com/">169.72</wtg:WeightTare>
  <wtg:WeightMax xmlns:wtg="https://www.wisetechglobal.com/">103.26</wtg:WeightMax>
  <wtg:Height xmlns:wtg="https://www.wisetechglobal.com/">86.62</wtg:Height>
  <wtg:Width xmlns:wtg="https://www.wisetechglobal.com/">87.98</wtg:Width>
</wtg:PrePackedBox>
```

