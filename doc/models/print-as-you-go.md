
# Print as You Go

Container element the Print As You Go option.

## Structure

`PrintAsYouGo`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Enabled` | `Boolean` | Optional | Used to determine if Print As You Go is active. | Boolean getEnabled() | setEnabled(Boolean enabled) |
| `MasterShipmentID` | `Integer` | Optional | The Shipment ID for the first package in the PAYG group.<br><br>**Default**: `0` | Integer getMasterShipmentID() | setMasterShipmentID(Integer masterShipmentID) |
| `CurrentPackageIndex` | `Integer` | Optional | The number of this package in the PAYG group.<br><br>**Default**: `0` | Integer getCurrentPackageIndex() | setCurrentPackageIndex(Integer currentPackageIndex) |
| `MaxPackageCount` | `Integer` | Optional | The number of packages in the PAYG group.<br><br>**Default**: `0` | Integer getMaxPackageCount() | setMaxPackageCount(Integer maxPackageCount) |

## Example (as XML)

```xml
<wtg:PrintAsYouGo xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:MasterShipmentID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:MasterShipmentID>
  <wtg:CurrentPackageIndex xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:CurrentPackageIndex>
  <wtg:MaxPackageCount xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:MaxPackageCount>
  <wtg:Enabled xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Enabled>
</wtg:PrintAsYouGo>
```

