
# Page

Container for an individual page to be printed by the caller of the transaction (client).

## Structure

`Page`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Url` | `String` | Optional | The address to access to contents of the page. | String getUrl() | setUrl(String url) |
| `Width` | `Integer` | Optional | The width in pixels of the page.<br><br>**Default**: `0` | Integer getWidth() | setWidth(Integer width) |
| `Height` | `Integer` | Optional | The height in pixels of the page.<br><br>**Default**: `0` | Integer getHeight() | setHeight(Integer height) |
| `UsePercentage` | `Boolean` | Optional | Indicates if the width and height values are expressed in percentages rather than pixels.<br><br>**Default**: `false` | Boolean getUsePercentage() | setUsePercentage(Boolean usePercentage) |

## Example (as XML)

```xml
<wtg:Page xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Width xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Width>
  <wtg:Height xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Height>
  <wtg:UsePercentage xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:UsePercentage>
  <wtg:Url xmlns:wtg="https://www.wisetechglobal.com/">Url2</wtg:Url>
</wtg:Page>
```

