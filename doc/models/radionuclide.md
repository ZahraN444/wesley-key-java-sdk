
# Radionuclide

Container for radionuclide details.

## Structure

`Radionuclide`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Name` | `String` | Optional | Name of substance. | String getName() | setName(String name) |
| `Activity` | `String` | Optional | Value indicates the radioactivity of this substance. | String getActivity() | setActivity(String activity) |
| `Measure` | `String` | Optional | Value indicates the unit of measure. | String getMeasure() | setMeasure(String measure) |
| `RadioactivePackagingType` | `String` | Optional | Value indicates the packaging type. | String getRadioactivePackagingType() | setRadioactivePackagingType(String radioactivePackagingType) |
| `TransportIndex` | `String` | Optional | Value indicates the transport index. | String getTransportIndex() | setTransportIndex(String transportIndex) |
| `RadioactiveLabelType` | `String` | Optional | The label type to use. | String getRadioactiveLabelType() | setRadioactiveLabelType(String radioactiveLabelType) |
| `SurfaceReading` | `Integer` | Optional | The surface reading for this substance.<br><br>**Default**: `0` | Integer getSurfaceReading() | setSurfaceReading(Integer surfaceReading) |
| `Length` | `Double` | Optional | Length of this substance.<br><br>**Default**: `0d` | Double getLength() | setLength(Double length) |
| `Width` | `Double` | Optional | Width of this substance.<br><br>**Default**: `0d` | Double getWidth() | setWidth(Double width) |
| `Height` | `Double` | Optional | Height of this substance.<br><br>**Default**: `0d` | Double getHeight() | setHeight(Double height) |
| `DimensionsUOM` | `String` | Optional | Unit of measure in use. | String getDimensionsUOM() | setDimensionsUOM(String dimensionsUOM) |
| `PhysicalForm` | `String` | Optional | Value indicates the physical form of this substance. | String getPhysicalForm() | setPhysicalForm(String physicalForm) |
| `ChemicalFormula` | `String` | Optional | Value indicates the chemical formula of this substance. | String getChemicalFormula() | setChemicalFormula(String chemicalFormula) |
| `ExceptedPackagesRadioactiveMaterialsIndicator` | `Integer` | Optional | Excepted packages radioactive materials indicator of the radionuclide<br><br>**Default**: `0` | Integer getExceptedPackagesRadioactiveMaterialsIndicator() | setExceptedPackagesRadioactiveMaterialsIndicator(Integer exceptedPackagesRadioactiveMaterialsIndicator) |
| `CriticalitySafetyIndex` | `Double` | Optional | Criticality safety index of the radionuclide<br><br>**Default**: `0d` | Double getCriticalitySafetyIndex() | setCriticalitySafetyIndex(Double criticalitySafetyIndex) |

## Example (as XML)

```xml
<wtg:Radionuclide xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:SurfaceReading xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:SurfaceReading>
  <wtg:Length xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Length>
  <wtg:Width xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Width>
  <wtg:Height xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Height>
  <wtg:ExceptedPackagesRadioactiveMaterialsIndicator xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ExceptedPackagesRadioactiveMaterialsIndicator>
  <wtg:CriticalitySafetyIndex xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:CriticalitySafetyIndex>
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name6</wtg:Name>
  <wtg:Activity xmlns:wtg="https://www.wisetechglobal.com/">Activity0</wtg:Activity>
  <wtg:Measure xmlns:wtg="https://www.wisetechglobal.com/">Measure2</wtg:Measure>
  <wtg:RadioactivePackagingType xmlns:wtg="https://www.wisetechglobal.com/">RadioactivePackagingType4</wtg:RadioactivePackagingType>
  <wtg:TransportIndex xmlns:wtg="https://www.wisetechglobal.com/">TransportIndex0</wtg:TransportIndex>
</wtg:Radionuclide>
```

