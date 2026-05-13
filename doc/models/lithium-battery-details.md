
# Lithium Battery Details

Outer container for Lithium Battery details for package.

## Structure

`LithiumBatteryDetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Material` | [`MaterialEnum`](../../doc/models/material-enum.md) | Optional | Describes the material composition of the battery or cell | MaterialEnum getMaterial() | setMaterial(MaterialEnum material) |
| `Packing` | [`PackingEnum`](../../doc/models/packing-enum.md) | Optional | Describes the packing arrangement of the battery or cell with respect to other items within the same package | PackingEnum getPacking() | setPacking(PackingEnum packing) |

## Example (as XML)

```xml
<wtg:LithiumBatteryDetails xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Material xmlns:wtg="https://www.wisetechglobal.com/">1</wtg:Material>
  <wtg:Packing xmlns:wtg="https://www.wisetechglobal.com/">1</wtg:Packing>
</wtg:LithiumBatteryDetails>
```

