
# Special Care

Outer container for special care details for package.

## Structure

`SpecialCare`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`TypeEnum`](../../doc/models/type-enum.md) | Optional | Describes the special care required | TypeEnum getType() | setType(TypeEnum type) |
| `Temperature` | [`TemperatureEnum`](../../doc/models/temperature-enum.md) | Optional | Describes the storage temperature for the special care package | TemperatureEnum getTemperature() | setTemperature(TemperatureEnum temperature) |
| `ExpediteMethod` | [`ExpediteMethodEnum`](../../doc/models/expedite-method-enum.md) | Optional | Describes the method used to expedite delivery of the special care package | ExpediteMethodEnum getExpediteMethod() | setExpediteMethod(ExpediteMethodEnum expediteMethod) |
| `Instructions` | [`InstructionsEnum`](../../doc/models/instructions-enum.md) | Optional | Describes the which contact method to be used to communicate problems delivering the special care package | InstructionsEnum getInstructions() | setInstructions(InstructionsEnum instructions) |
| `ReturnToShipper` | `Boolean` | Optional | Indicates whether a special care package should be returned to shipper if problems arise.<br><br>**Default**: `false` | Boolean getReturnToShipper() | setReturnToShipper(Boolean returnToShipper) |
| `PackageIdentifier` | `String` | Optional | The identifier of the attached tracking device. | String getPackageIdentifier() | setPackageIdentifier(String packageIdentifier) |

## Example (as XML)

```xml
<wtg:SpecialCare xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ReturnToShipper xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReturnToShipper>
  <wtg:Type xmlns:wtg="https://www.wisetechglobal.com/">1</wtg:Type>
  <wtg:Temperature xmlns:wtg="https://www.wisetechglobal.com/">1</wtg:Temperature>
  <wtg:ExpediteMethod xmlns:wtg="https://www.wisetechglobal.com/">128</wtg:ExpediteMethod>
  <wtg:Instructions xmlns:wtg="https://www.wisetechglobal.com/">512</wtg:Instructions>
</wtg:SpecialCare>
```

