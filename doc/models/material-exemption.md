
# Material Exemption

Container for material exemption.

## Structure

`MaterialExemption`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ExemptionName` | `String` | Required | Hazardous material exemption name for 3rd party hazardous partner. | String getExemptionName() | setExemptionName(String exemptionName) |
| `ExemptionType` | [`ExemptionTypeEnum`](../../doc/models/exemption-type-enum.md) | Required | Hazardous material exemption type for 3rd party hazardous partner. | ExemptionTypeEnum getExemptionType() | setExemptionType(ExemptionTypeEnum exemptionType) |

## Example (as XML)

```xml
<wtg:MaterialExemption xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ExemptionName xmlns:wtg="https://www.wisetechglobal.com/">ExemptionName2</wtg:ExemptionName>
  <wtg:ExemptionType xmlns:wtg="https://www.wisetechglobal.com/">CA</wtg:ExemptionType>
</wtg:MaterialExemption>
```

