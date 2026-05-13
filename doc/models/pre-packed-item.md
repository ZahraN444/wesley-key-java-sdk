
# Pre Packed Item

## Structure

`PrePackedItem`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ItemDescription` | `String` | Optional | Maps to paccurate "name" property: Name or description of item for your reference. | String getItemDescription() | setItemDescription(String itemDescription) |
| `Color` | `String` | Optional | designated color name for the item in pack visualizations. | String getColor() | setColor(String color) |
| `Weight` | `Double` | Optional | Item weight | Double getWeight() | setWeight(Double weight) |
| `Virtual` | `Boolean` | Optional | Whether or not this is a real item or a virtual, blocking space (from a subspace or loading rules) | Boolean getVirtual() | setVirtual(Boolean virtual) |
| `Height` | `Double` | Optional | Height of the content. | Double getHeight() | setHeight(Double height) |
| `Width` | `Double` | Optional | Width of the content. | Double getWidth() | setWidth(Double width) |
| `Length` | `Double` | Optional | Length of the content. | Double getLength() | setLength(Double length) |
| `CenterOfMass` | [`Point`](../../doc/models/point.md) | Optional | 3-dimensional Coordinates of the packed item's center of mass | Point getCenterOfMass() | setCenterOfMass(Point centerOfMass) |
| `Origin` | [`Point`](../../doc/models/point.md) | Optional | Origin of the packed item, relative to the box in which is is packed | Point getOrigin() | setOrigin(Point origin) |

## Example (as XML)

```xml
<wtg:PrePackedItem xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ItemDescription xmlns:wtg="https://www.wisetechglobal.com/">ItemDescription6</wtg:ItemDescription>
  <wtg:Color xmlns:wtg="https://www.wisetechglobal.com/">Color0</wtg:Color>
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">221.78</wtg:Weight>
  <wtg:Virtual xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Virtual>
  <wtg:Height xmlns:wtg="https://www.wisetechglobal.com/">70.14</wtg:Height>
</wtg:PrePackedItem>
```

