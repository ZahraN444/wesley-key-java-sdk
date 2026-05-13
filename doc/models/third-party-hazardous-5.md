
# Third Party Hazardous 5

Container for details for processing by an external hazardous compliance system.

## Structure

`ThirdPartyHazardous5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `UseThirdPartyHazardous` | `Boolean` | Optional | Indicates if the shipment was created using a third party hazardous package.<br><br>**Default**: `false` | Boolean getUseThirdPartyHazardous() | setUseThirdPartyHazardous(Boolean useThirdPartyHazardous) |
| `CarrierID` | `String` | Required | Numeric identifier for the carrier. | String getCarrierID() | setCarrierID(String carrierID) |
| `SessionID` | `String` | Optional | Third Party Hazardous Session Identifier. | String getSessionID() | setSessionID(String sessionID) |
| `PackageID` | `Integer` | Optional | Third Party Hazardous Package Identifier.<br><br>**Default**: `0` | Integer getPackageID() | setPackageID(Integer packageID) |
| `PackageUri` | `String` | Optional | Third Party Hazardous Package Uri. | String getPackageUri() | setPackageUri(String packageUri) |
| `ShipmentKey` | `String` | Required | Third Party Hazardous Shipment Key. | String getShipmentKey() | setShipmentKey(String shipmentKey) |

## Example (as XML)

```xml
<wtg:ThirdPartyHazardous xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:UseThirdPartyHazardous xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:UseThirdPartyHazardous>
  <wtg:CarrierID xmlns:wtg="https://www.wisetechglobal.com/"></wtg:CarrierID>
  <wtg:PackageID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageID>
  <wtg:ShipmentKey xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ShipmentKey>
  <wtg:SessionID xmlns:wtg="https://www.wisetechglobal.com/">SessionID8</wtg:SessionID>
  <wtg:PackageUri xmlns:wtg="https://www.wisetechglobal.com/">PackageUri0</wtg:PackageUri>
</wtg:ThirdPartyHazardous>
```

