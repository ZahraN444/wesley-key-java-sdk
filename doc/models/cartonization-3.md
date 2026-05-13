
# Cartonization 3

Container for cartonization data for this transaction.

## Structure

`Cartonization3`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `CartonizationGroupID` | `Integer` | Optional | Numeric identifier for a cartonization group.<br><br>**Default**: `0` | Integer getCartonizationGroupID() | setCartonizationGroupID(Integer cartonizationGroupID) |
| `SVGData` | `String` | Optional | Html that contains the visualization web page that represents the cartonized items. | String getSVGData() | setSVGData(String sVGData) |
| `JSONBoxData` | `String` | Optional | Html that contains the json data that represents the cartonized items. | String getJSONBoxData() | setJSONBoxData(String jSONBoxData) |
| `Packages` | [`Packages9`](../../doc/models/packages-9.md) | Optional | Container for all packages associated with the transaction. | Packages9 getPackages() | setPackages(Packages9 packages) |

## Example (as XML)

```xml
<wtg:Cartonization xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:CartonizationGroupID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:CartonizationGroupID>
  <wtg:SVGData xmlns:wtg="https://www.wisetechglobal.com/">SVGData6</wtg:SVGData>
  <wtg:JSONBoxData xmlns:wtg="https://www.wisetechglobal.com/">JSONBoxData6</wtg:JSONBoxData>
  <wtg:Packages xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Packages>
</wtg:Cartonization>
```

