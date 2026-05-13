
# Material 3

Container for material details.

## Structure

`Material3`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Radionuclide` | [`Radionuclide`](../../doc/models/radionuclide.md) | Optional | Container for radionuclide details. | Radionuclide getRadionuclide() | setRadionuclide(Radionuclide radionuclide) |
| `Hazardous` | `Boolean` | Optional | Indicates whether the line item is hazardous.  Defaults to not hazardous if omitted.<br><br>**Default**: `false` | Boolean getHazardous() | setHazardous(Boolean hazardous) |
| `HazardousIdentifier` | `String` | Optional | Hazardous Material Identification Number for the line item. | String getHazardousIdentifier() | setHazardousIdentifier(String hazardousIdentifier) |
| `HazardousProperShippingName` | `String` | Optional | Proper Shipping Name for the line item. | String getHazardousProperShippingName() | setHazardousProperShippingName(String hazardousProperShippingName) |
| `HazardousTotalQuantity` | `Double` | Optional | Total Material Quantity.<br><br>**Default**: `0d` | Double getHazardousTotalQuantity() | setHazardousTotalQuantity(Double hazardousTotalQuantity) |
| `HazardousTechnicalName` | `String` | Optional | Technical Name for the line item. | String getHazardousTechnicalName() | setHazardousTechnicalName(String hazardousTechnicalName) |
| `NumberOfInnerContainers` | `Integer` | Optional | The number of items packed inside the content item.<br><br>**Default**: `0` | Integer getNumberOfInnerContainers() | setNumberOfInnerContainers(Integer numberOfInnerContainers) |
| `HazardousAccessible` | `Boolean` | Optional | Indicates whether the hazardous line item must remain accessible during transportation.  Defaults to not accessible if omitted.<br><br>**Default**: `false` | Boolean getHazardousAccessible() | setHazardousAccessible(Boolean hazardousAccessible) |
| `HazardousPassengerAircraft` | `Boolean` | Optional | Indicates whether the hazardous line item can be transported on a passenger aircraft.  Defaults to cannot be transported on a passenger aircraft if omitted.<br><br>**Default**: `false` | Boolean getHazardousPassengerAircraft() | setHazardousPassengerAircraft(Boolean hazardousPassengerAircraft) |
| `HazardousCargoAircraftOnly` | `Boolean` | Optional | Indicates whether the hazardous line item can only be transported on a cargo aircraft.  Defaults to not cargo aircraft only if omitted.<br><br>**Default**: `false` | Boolean getHazardousCargoAircraftOnly() | setHazardousCargoAircraftOnly(Boolean hazardousCargoAircraftOnly) |
| `HazardousRequiredInformation` | `String` | Optional | Any additional required information relating to the hazardous item, e.g. Limited Qty, permit numbers and type. | String getHazardousRequiredInformation() | setHazardousRequiredInformation(String hazardousRequiredInformation) |
| `HazardousLabelCodes` | `String` | Optional | Hazardous Label Codes for the line item. | String getHazardousLabelCodes() | setHazardousLabelCodes(String hazardousLabelCodes) |
| `HazardousAirLabels` | `String` | Optional | Hazardous Air Labels for the line item. | String getHazardousAirLabels() | setHazardousAirLabels(String hazardousAirLabels) |
| `HazardousPackingInstructions` | `String` | Optional | Hazardous packing instructions for the product. | String getHazardousPackingInstructions() | setHazardousPackingInstructions(String hazardousPackingInstructions) |
| `HazardousSubClass` | `String` | Optional | Hazardous Sub-Class for the line item. | String getHazardousSubClass() | setHazardousSubClass(String hazardousSubClass) |
| `HazardousPackingGroup` | `String` | Optional | Hazardous Packing Group for the line item. | String getHazardousPackingGroup() | setHazardousPackingGroup(String hazardousPackingGroup) |
| `HazardousSpecialProvision` | `String` | Optional | Value indicates the hazardous special provision in use. | String getHazardousSpecialProvision() | setHazardousSpecialProvision(String hazardousSpecialProvision) |
| `HazardousClass` | `String` | Optional | Hazardous Class for the line item. | String getHazardousClass() | setHazardousClass(String hazardousClass) |
| `HazardousLabels` | `String` | Optional | Hazardous Labels for the line item. | String getHazardousLabels() | setHazardousLabels(String hazardousLabels) |
| `HazardousConcentration` | `Integer` | Optional | The percentage concentration for the line item.<br><br>**Default**: `0` | Integer getHazardousConcentration() | setHazardousConcentration(Integer hazardousConcentration) |
| `Quantity` | `Double` | Optional | Material Quantity.<br><br>**Default**: `0d` | Double getQuantity() | setQuantity(Double quantity) |
| `QuantityUOM` | `String` | Optional | The units of measure for the material quantity. | String getQuantityUOM() | setQuantityUOM(String quantityUOM) |
| `Weight` | `Double` | Optional | Material Weight.<br><br>**Default**: `0d` | Double getWeight() | setWeight(Double weight) |
| `WeightUOM` | `String` | Optional | The units of measure for the material weight. | String getWeightUOM() | setWeightUOM(String weightUOM) |
| `NetMassQuantity` | `Double` | Optional | Net mass quantity.<br><br>**Default**: `0d` | Double getNetMassQuantity() | setNetMassQuantity(Double netMassQuantity) |
| `NetMassUOM` | `String` | Optional | Net mass units of measure. | String getNetMassUOM() | setNetMassUOM(String netMassUOM) |
| `NetExplosive` | [`NetExplosive`](../../doc/models/net-explosive.md) | Optional | Container for net explosive details. | NetExplosive getNetExplosive() | setNetExplosive(NetExplosive netExplosive) |
| `MaterialKey` | `String` | Optional | Hazardous material key for the product for 3rd party hazardous partner. | String getMaterialKey() | setMaterialKey(String materialKey) |
| `NameKey` | `String` | Optional | Hazardous name key for the product for 3rd party hazardous partner. | String getNameKey() | setNameKey(String nameKey) |
| `InnerPackagingType` | `String` | Optional | Hazardous inner packaging type for the product for 3rd party hazardous partner. | String getInnerPackagingType() | setInnerPackagingType(String innerPackagingType) |
| `PackageInstructionType` | `String` | Optional | Hazardous packaging instruction type for the product for 3rd party hazardous partner. | String getPackageInstructionType() | setPackageInstructionType(String packageInstructionType) |
| `ReportableQuantity` | `Boolean` | Optional | Hazardous product quantity is reportable for 3rd party hazardous partner.<br><br>**Default**: `false` | Boolean getReportableQuantity() | setReportableQuantity(Boolean reportableQuantity) |
| `ConsumerCommodity` | `Boolean` | Optional | Material is classified as Consumer Commodity (ORM-D).<br><br>**Default**: `false` | Boolean getConsumerCommodity() | setConsumerCommodity(Boolean consumerCommodity) |
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
| `MaterialExemptions` | [`MaterialExemptions`](../../doc/models/material-exemptions.md) | Optional | Container for material exemptions. | MaterialExemptions getMaterialExemptions() | setMaterialExemptions(MaterialExemptions materialExemptions) |

## Example (as XML)

```xml
<wtg:Material xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Hazardous xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Hazardous>
  <wtg:HazardousTotalQuantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:HazardousTotalQuantity>
  <wtg:NumberOfInnerContainers xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:NumberOfInnerContainers>
  <wtg:HazardousAccessible xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HazardousAccessible>
  <wtg:HazardousPassengerAircraft xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HazardousPassengerAircraft>
  <wtg:HazardousCargoAircraftOnly xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HazardousCargoAircraftOnly>
  <wtg:HazardousConcentration xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:HazardousConcentration>
  <wtg:Quantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Quantity>
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Weight>
  <wtg:NetMassQuantity xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:NetMassQuantity>
  <wtg:ReportableQuantity xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReportableQuantity>
  <wtg:ConsumerCommodity xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ConsumerCommodity>
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
  <wtg:Radionuclide xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Radionuclide>
  <wtg:HazardousIdentifier xmlns:wtg="https://www.wisetechglobal.com/">HazardousIdentifier4</wtg:HazardousIdentifier>
  <wtg:HazardousProperShippingName xmlns:wtg="https://www.wisetechglobal.com/">HazardousProperShippingName2</wtg:HazardousProperShippingName>
</wtg:Material>
```

