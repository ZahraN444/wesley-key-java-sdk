
# Third Party Hazardous 4

Container for details for processing by an external hazardous compliance system.

## Structure

`ThirdPartyHazardous4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Materials` | [`Materials2`](../../doc/models/materials-2.md) | Optional | Container for all material details. | Materials2 getMaterials() | setMaterials(Materials2 materials) |
| `MaterialKey` | `String` | Optional | Hazardous material key for the product for 3rd party hazardous partner. | String getMaterialKey() | setMaterialKey(String materialKey) |
| `NameKey` | `String` | Optional | Hazardous name key for the product for 3rd party hazardous partner. | String getNameKey() | setNameKey(String nameKey) |
| `InnerPackagingType` | `String` | Optional | Hazardous inner packaging type for the product for 3rd party hazardous partner. | String getInnerPackagingType() | setInnerPackagingType(String innerPackagingType) |
| `PackageInstructionType` | `String` | Optional | Hazardous packaging instruction type for the product for 3rd party hazardous partner. | String getPackageInstructionType() | setPackageInstructionType(String packageInstructionType) |
| `ReportableQuantity` | `Boolean` | Optional | Hazardous product quantity is reportable for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getReportableQuantity() | setReportableQuantity(Boolean reportableQuantity) |
| `Mixture` | `Boolean` | Optional | Hazardous product is mixture for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getMixture() | setMixture(Boolean mixture) |
| `Solution` | `Boolean` | Optional | Hazardous product is solution for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getSolution() | setSolution(Boolean solution) |
| `Solid` | `Boolean` | Optional | Hazardous product is solid for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getSolid() | setSolid(Boolean solid) |
| `Molten` | `Boolean` | Optional | Hazardous product is molten for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getMolten() | setMolten(Boolean molten) |
| `Liquid` | `Boolean` | Optional | Hazardous product is liquid for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getLiquid() | setLiquid(Boolean liquid) |
| `Stabilized` | `Boolean` | Optional | Hazardous product is stabilized for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getStabilized() | setStabilized(Boolean stabilized) |
| `Waste` | `Boolean` | Optional | Hazardous product is waste for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getWaste() | setWaste(Boolean waste) |
| `Hot` | `Boolean` | Optional | Hazardous product is hot for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getHot() | setHot(Boolean hot) |
| `MarinePollutant` | `Boolean` | Optional | Hazardous product is a marine pollutant for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getMarinePollutant() | setMarinePollutant(Boolean marinePollutant) |
| `MaritimeOnly` | `Boolean` | Optional | Hazardous product is a maritime only for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getMaritimeOnly() | setMaritimeOnly(Boolean maritimeOnly) |
| `ElevatedTemperature` | `Boolean` | Optional | Hazardous productis at elevated temperature for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getElevatedTemperature() | setElevatedTemperature(Boolean elevatedTemperature) |
| `Empty` | `Boolean` | Optional | Hazardous product container is empty for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getEmpty() | setEmpty(Boolean empty) |
| `IsMaterialNonHazmat` | `Boolean` | Optional | Marks material as NonHazardous for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getIsMaterialNonHazmat() | setIsMaterialNonHazmat(Boolean isMaterialNonHazmat) |
| `IsMaterialNotInPackage` | `Boolean` | Optional | Hazardous product not packaged for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getIsMaterialNotInPackage() | setIsMaterialNotInPackage(Boolean isMaterialNotInPackage) |
| `IsInnerPackagingLiquid` | `Boolean` | Optional | Hazardous product is in liquid packaging for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getIsInnerPackagingLiquid() | setIsInnerPackagingLiquid(Boolean isInnerPackagingLiquid) |
| `ShowMarinePollutantLabel` | `Boolean` | Optional | Hazardous product show marine pollutant label for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getShowMarinePollutantLabel() | setShowMarinePollutantLabel(Boolean showMarinePollutantLabel) |
| `ShowOrientationLabel` | `Boolean` | Optional | Show orientation label for hazardous product for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getShowOrientationLabel() | setShowOrientationLabel(Boolean showOrientationLabel) |
| `CustomInnerPackagingType` | `String` | Optional | Custom inner packaging type for Hazardous product for 3rd party hazardous partner. | String getCustomInnerPackagingType() | setCustomInnerPackagingType(String customInnerPackagingType) |
| `Authorization` | `String` | Optional | Hazardous Authorization for the product for 3rd party hazardous partner. | String getAuthorization() | setAuthorization(String authorization) |
| `ErgNumber` | `String` | Optional | Hazardous ErgNumber for the product for 3rd party hazardous partner. | String getErgNumber() | setErgNumber(String ergNumber) |
| `AdditionalQuantityInformation` | `String` | Optional | Hazardous additional quantity information for the product for 3rd party hazardous partner. | String getAdditionalQuantityInformation() | setAdditionalQuantityInformation(String additionalQuantityInformation) |
| `ToxicInhalationHazardZone` | `String` | Optional | Toxic Inhalation Hazard Zone for the product for 3rd party hazardous partner. | String getToxicInhalationHazardZone() | setToxicInhalationHazardZone(String toxicInhalationHazardZone) |
| `OtherRequiredInformation` | `String` | Optional | Other required information for hazardous product for 3rd party hazardous partner. | String getOtherRequiredInformation() | setOtherRequiredInformation(String otherRequiredInformation) |
| `EmptyPackageType` | `String` | Optional | Empty package type for hazardous product for 3rd party hazardous partner. | String getEmptyPackageType() | setEmptyPackageType(String emptyPackageType) |

## Example (as XML)

```xml
<wtg:ThirdPartyHazardous xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ReportableQuantity xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReportableQuantity>
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
  <wtg:MaterialKey xmlns:wtg="https://www.wisetechglobal.com/">MaterialKey4</wtg:MaterialKey>
  <wtg:NameKey xmlns:wtg="https://www.wisetechglobal.com/">NameKey2</wtg:NameKey>
  <wtg:InnerPackagingType xmlns:wtg="https://www.wisetechglobal.com/">InnerPackagingType4</wtg:InnerPackagingType>
  <wtg:PackageInstructionType xmlns:wtg="https://www.wisetechglobal.com/">PackageInstructionType0</wtg:PackageInstructionType>
</wtg:ThirdPartyHazardous>
```

