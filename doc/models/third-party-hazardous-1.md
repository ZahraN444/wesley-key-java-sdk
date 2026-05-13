
# Third Party Hazardous 1

Container for details for processing by an external hazardous compliance system.

## Structure

`ThirdPartyHazardous1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Materials` | [`Materials`](../../doc/models/materials.md) | Optional | Container for all material details. | Materials getMaterials() | setMaterials(Materials materials) |
| `MaterialKey` | `String` | Optional | Hazardous name key for the product for 3rd party hazardous partner. | String getMaterialKey() | setMaterialKey(String materialKey) |
| `NameKey` | `String` | Optional | Hazardous name key for the product for 3rd party hazardous partner. | String getNameKey() | setNameKey(String nameKey) |
| `InnerPackagingType` | `String` | Optional | Hazardous name key for the product for 3rd party hazardous partner. | String getInnerPackagingType() | setInnerPackagingType(String innerPackagingType) |
| `PackageInstructionType` | `String` | Optional | Hazardous name key for the product for 3rd party hazardous partner. | String getPackageInstructionType() | setPackageInstructionType(String packageInstructionType) |
| `ReportableQuantity` | `String` | Optional | Hazardous name key for the product for 3rd party hazardous partner. | String getReportableQuantity() | setReportableQuantity(String reportableQuantity) |
| `Mixture` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getMixture() | setMixture(Boolean mixture) |
| `Solution` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getSolution() | setSolution(Boolean solution) |
| `Solid` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getSolid() | setSolid(Boolean solid) |
| `Molten` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getMolten() | setMolten(Boolean molten) |
| `Liquid` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getLiquid() | setLiquid(Boolean liquid) |
| `Stabilized` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getStabilized() | setStabilized(Boolean stabilized) |
| `Waste` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getWaste() | setWaste(Boolean waste) |
| `Hot` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getHot() | setHot(Boolean hot) |
| `MarinePollutant` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getMarinePollutant() | setMarinePollutant(Boolean marinePollutant) |
| `MaritimeOnly` | `Boolean` | Optional | Hazardous product is a maritime only for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getMaritimeOnly() | setMaritimeOnly(Boolean maritimeOnly) |
| `ElevatedTemperature` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getElevatedTemperature() | setElevatedTemperature(Boolean elevatedTemperature) |
| `Empty` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getEmpty() | setEmpty(Boolean empty) |
| `IsMaterialNonHazmat` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getIsMaterialNonHazmat() | setIsMaterialNonHazmat(Boolean isMaterialNonHazmat) |
| `IsMaterialNotInPackage` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getIsMaterialNotInPackage() | setIsMaterialNotInPackage(Boolean isMaterialNotInPackage) |
| `IsInnerPackagingLiquid` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getIsInnerPackagingLiquid() | setIsInnerPackagingLiquid(Boolean isInnerPackagingLiquid) |
| `ShowMarinePollutantLabel` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getShowMarinePollutantLabel() | setShowMarinePollutantLabel(Boolean showMarinePollutantLabel) |
| `ShowOrientationLabel` | `Boolean` | Optional | Hazardous name key for the product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getShowOrientationLabel() | setShowOrientationLabel(Boolean showOrientationLabel) |
| `CustomInnerPackagingType` | `String` | Optional | Hazardous name key for the product for 3rd party hazardous partner. | String getCustomInnerPackagingType() | setCustomInnerPackagingType(String customInnerPackagingType) |
| `Authorization` | `String` | Optional | Hazardous name key for the product for 3rd party hazardous partner. | String getAuthorization() | setAuthorization(String authorization) |
| `ErgNumber` | `String` | Optional | Hazardous name key for the product for 3rd party hazardous partner. | String getErgNumber() | setErgNumber(String ergNumber) |
| `AdditionalQuantityInformation` | `String` | Optional | Hazardous name key for the product for 3rd party hazardous partner. | String getAdditionalQuantityInformation() | setAdditionalQuantityInformation(String additionalQuantityInformation) |
| `ToxicInhalationHazardZone` | `String` | Optional | Toxic Inhalation Hazard Zone for the product for 3rd party hazardous partner. | String getToxicInhalationHazardZone() | setToxicInhalationHazardZone(String toxicInhalationHazardZone) |
| `OtherRequiredInformation` | `String` | Optional | Other required information for hazardous product for 3rd party hazardous partner. | String getOtherRequiredInformation() | setOtherRequiredInformation(String otherRequiredInformation) |
| `EmptyPackageType` | `String` | Optional | Hazardous name key for the product for 3rd party hazardous partner. | String getEmptyPackageType() | setEmptyPackageType(String emptyPackageType) |

## Example (as XML)

```xml
<wtg:ThirdPartyHazardous xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Mixture xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Mixture>
  <wtg:Solution xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Solution>
  <wtg:Solid xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Solid>
  <wtg:Molten xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Molten>
  <wtg:Liquid xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Liquid>
  <wtg:Stabilized xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Stabilized>
  <wtg:Waste xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Waste>
  <wtg:Hot xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Hot>
  <wtg:MarinePollutant xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:MarinePollutant>
  <wtg:MaritimeOnly xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:MaritimeOnly>
  <wtg:ElevatedTemperature xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ElevatedTemperature>
  <wtg:Empty xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Empty>
  <wtg:IsMaterialNonHazmat xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:IsMaterialNonHazmat>
  <wtg:IsMaterialNotInPackage xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:IsMaterialNotInPackage>
  <wtg:IsInnerPackagingLiquid xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:IsInnerPackagingLiquid>
  <wtg:ShowMarinePollutantLabel xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ShowMarinePollutantLabel>
  <wtg:ShowOrientationLabel xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ShowOrientationLabel>
  <wtg:Materials xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Materials>
  <wtg:MaterialKey xmlns:wtg="https://www.wisetechglobal.com/">MaterialKey2</wtg:MaterialKey>
  <wtg:NameKey xmlns:wtg="https://www.wisetechglobal.com/">NameKey0</wtg:NameKey>
  <wtg:InnerPackagingType xmlns:wtg="https://www.wisetechglobal.com/">InnerPackagingType2</wtg:InnerPackagingType>
  <wtg:PackageInstructionType xmlns:wtg="https://www.wisetechglobal.com/">PackageInstructionType8</wtg:PackageInstructionType>
</wtg:ThirdPartyHazardous>
```

