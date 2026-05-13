
# Pierbridge Address Validation Request

Validates a postal address using a carrier based validation system.

## Structure

`PierbridgeAddressValidationRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TransactionIdentifier` | `String` | Optional | A unique identifier for the transaction, this value is not used during processing and will be returned in the response. | String getTransactionIdentifier() | setTransactionIdentifier(String transactionIdentifier) |
| `ControlIdentifier` | `String` | Optional | A reference to a control which generated the request, this value is not used during processing and will be returned in the response. | String getControlIdentifier() | setControlIdentifier(String controlIdentifier) |
| `UserName` | `String` | Required | The user name to use when processing the transaction.<br><br>**Constraints**: *Minimum Length*: `1` | String getUserName() | setUserName(String userName) |
| `Carrier` | `Integer` | Optional | Numeric identifier for the carrier.<br><br>**Default**: `0` | Integer getCarrier() | setCarrier(Integer carrier) |
| `Live` | `Boolean` | Optional | Indicates whether the transaction is a test or live.  Defaults to system configured value if not submitted.<br><br>**Default**: `false` | Boolean getLive() | setLive(Boolean live) |
| `Address` | [`Address`](../../doc/models/address.md) | Required | Container for an address. | Address getAddress() | setAddress(Address address) |
| `PersonalShipping` | [`PersonalShipping`](../../doc/models/personal-shipping.md) | Optional | Container for personal shipping elements. | PersonalShipping getPersonalShipping() | setPersonalShipping(PersonalShipping personalShipping) |
| `Diagnostics` | [`Diagnostics`](../../doc/models/diagnostics.md) | Optional | Container for logging and diagnostic override elements. | Diagnostics getDiagnostics() | setDiagnostics(Diagnostics diagnostics) |
| `Identification` | [`Identification`](../../doc/models/identification.md) | Optional | Container for client identification elements. | Identification getIdentification() | setIdentification(Identification identification) |

## Example (as XML)

```xml
<wtg:PierbridgeAddressValidationRequest xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:UserName xmlns:wtg="https://www.wisetechglobal.com/"></wtg:UserName>
  <wtg:Carrier xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Carrier>
  <wtg:Live xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Live>
  <wtg:Address xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:Street></wtg:Street>
    <wtg:City></wtg:City>
    <wtg:Region></wtg:Region>
    <wtg:PostalCode></wtg:PostalCode>
    <wtg:Country></wtg:Country>
    <wtg:Residential>false</wtg:Residential>
    <wtg:CompanyName>CompanyName8</wtg:CompanyName>
    <wtg:Locale>Locale0</wtg:Locale>
    <wtg:Other>Other0</wtg:Other>
    <wtg:RegionName>RegionName4</wtg:RegionName>
    <wtg:CountryName>CountryName4</wtg:CountryName>
  </wtg:Address>
  <wtg:TransactionIdentifier xmlns:wtg="https://www.wisetechglobal.com/">TransactionIdentifier2</wtg:TransactionIdentifier>
  <wtg:ControlIdentifier xmlns:wtg="https://www.wisetechglobal.com/">ControlIdentifier2</wtg:ControlIdentifier>
  <wtg:PersonalShipping xmlns:wtg="https://www.wisetechglobal.com/"></wtg:PersonalShipping>
</wtg:PierbridgeAddressValidationRequest>
```

