
# Package Type

Container element for the carrier package type.

## Structure

`PackageType`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ID` | `int` | Required | Numeric identifier for the carrier package type. | int getID() | setID(int iD) |
| `Description` | `String` | Optional | The name for the carrier package type. | String getDescription() | setDescription(String description) |

## Example (as XML)

```xml
<wtg:PackageType xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ID xmlns:wtg="https://www.wisetechglobal.com/">54</wtg:ID>
  <wtg:Description xmlns:wtg="https://www.wisetechglobal.com/">Description4</wtg:Description>
</wtg:PackageType>
```

