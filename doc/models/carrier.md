
# Carrier

Container element for the carrier.

## Structure

`Carrier`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ID` | `int` | Required | Numeric identifier for the carrier. | int getID() | setID(int iD) |
| `SystemCarrierName` | `String` | Optional | The system name for the carrier. | String getSystemCarrierName() | setSystemCarrierName(String systemCarrierName) |
| `Description` | `String` | Optional | The name for the carrier. | String getDescription() | setDescription(String description) |
| `SCAC` | `String` | Optional | The NMFTA (National Motor Freight Traffic Association) Standard Carrier Alpha Code of the carrier. | String getSCAC() | setSCAC(String sCAC) |
| `ExternalCarrierIdentifier` | `String` | Optional | An identifier for an external system associated with the carrier. | String getExternalCarrierIdentifier() | setExternalCarrierIdentifier(String externalCarrierIdentifier) |
| `ExternalServiceIdentifier` | `String` | Optional | An identifier for an external system associated with the carrier service. | String getExternalServiceIdentifier() | setExternalServiceIdentifier(String externalServiceIdentifier) |

## Example (as XML)

```xml
<wtg:Carrier xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ID xmlns:wtg="https://www.wisetechglobal.com/">144</wtg:ID>
  <wtg:SystemCarrierName xmlns:wtg="https://www.wisetechglobal.com/">SystemCarrierName0</wtg:SystemCarrierName>
  <wtg:Description xmlns:wtg="https://www.wisetechglobal.com/">Description0</wtg:Description>
  <wtg:SCAC xmlns:wtg="https://www.wisetechglobal.com/">SCAC4</wtg:SCAC>
  <wtg:ExternalCarrierIdentifier xmlns:wtg="https://www.wisetechglobal.com/">ExternalCarrierIdentifier0</wtg:ExternalCarrierIdentifier>
  <wtg:ExternalServiceIdentifier xmlns:wtg="https://www.wisetechglobal.com/">ExternalServiceIdentifier6</wtg:ExternalServiceIdentifier>
</wtg:Carrier>
```

