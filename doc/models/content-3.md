
# Content 3

Container for a individual content (line item) associated with the transaction.

## Structure

`Content3`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ContentRefNumber` | `String` | Required | Unique reference number for the content. | String getContentRefNumber() | setContentRefNumber(String contentRefNumber) |
| `Quantity` | `Double` | Optional | Quantity of the line item in the package.<br><br>**Default**: `0d` | Double getQuantity() | setQuantity(Double quantity) |
| `Value` | `Double` | Optional | Monetary value of a single line item.<br><br>**Default**: `0d` | Double getValue() | setValue(Double value) |
| `Weight` | `Double` | Optional | Weight of a single line item.<br><br>**Default**: `0d` | Double getWeight() | setWeight(Double weight) |
| `Length` | `Double` | Optional | Length of this line item.<br><br>**Default**: `0d` | Double getLength() | setLength(Double length) |
| `Width` | `Double` | Optional | Width of this line item.<br><br>**Default**: `0d` | Double getWidth() | setWidth(Double width) |
| `Height` | `Double` | Optional | Height of this line item.<br><br>**Default**: `0d` | Double getHeight() | setHeight(Double height) |
| `Description` | `String` | Optional | Description of the line item. | String getDescription() | setDescription(String description) |

## Example (as XML)

```xml
<wtg:Content xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ContentRefNumber xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ContentRefNumber>
  <wtg:Quantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Quantity>
  <wtg:Value xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Value>
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Weight>
  <wtg:Length xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Length>
  <wtg:Width xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Width>
  <wtg:Height xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Height>
</wtg:Content>
```

