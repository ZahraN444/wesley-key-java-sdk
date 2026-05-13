
# Service Type

Container element for the carrier service.

## Structure

`ServiceType`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ID` | `Integer` | Optional | Numeric identifier for the carrier service. | Integer getID() | setID(Integer iD) |
| `Description` | `String` | Optional | The name for the carrier service. | String getDescription() | setDescription(String description) |
| `IsGuaranteed` | `Boolean` | Optional | Indicates if the carrier service has a guaranteed delivery window.<br><br>**Default**: `false` | Boolean getIsGuaranteed() | setIsGuaranteed(Boolean isGuaranteed) |

## Example (as XML)

```xml
<wtg:ServiceType xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:IsGuaranteed xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:IsGuaranteed>
  <wtg:ID xmlns:wtg="https://www.wisetechglobal.com/">4</wtg:ID>
  <wtg:Description xmlns:wtg="https://www.wisetechglobal.com/">Description0</wtg:Description>
</wtg:ServiceType>
```

