
# Corrected Receiver Address

Container for the receiver address returned by the carrier if address corrections have been made.

## Structure

`CorrectedReceiverAddress`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Street` | `String` | Optional | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Optional | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address. | String getCountry() | setCountry(String country) |
| `Residential` | `Boolean` | Optional | Indicates whether the address is residential or commercial.<br><br>**Default**: `false` | Boolean getResidential() | setResidential(Boolean residential) |

## Example (as XML)

```xml
<wtg:CorrectedReceiverAddress xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Residential xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Residential>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street8</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale2</wtg:Locale>
  <wtg:Other xmlns:wtg="https://www.wisetechglobal.com/">Other2</wtg:Other>
  <wtg:City xmlns:wtg="https://www.wisetechglobal.com/">City2</wtg:City>
  <wtg:Region xmlns:wtg="https://www.wisetechglobal.com/">Region0</wtg:Region>
</wtg:CorrectedReceiverAddress>
```

