
# Address

Container for an address.

## Structure

`Address`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Required | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Required | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Required | The state or region of the address. | String getRegion() | setRegion(String region) |
| `RegionName` | `String` | Optional | The name of the region associated with the address, this value will be automatically added if available. | String getRegionName() | setRegionName(String regionName) |
| `PostalCode` | `String` | Required | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Required | The country code for the address. | String getCountry() | setCountry(String country) |
| `CountryName` | `String` | Optional | The name of the country associated with the address, this value will be automatically added if available. | String getCountryName() | setCountryName(String countryName) |
| `Residential` | `Boolean` | Optional | Indicates whether the address is residential or commercial.<br><br>**Default**: `false` | Boolean getResidential() | setResidential(Boolean residential) |

## Example (as XML)

```xml
<wtg:Address xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Street>
  <wtg:City xmlns:wtg="https://www.wisetechglobal.com/"></wtg:City>
  <wtg:Region xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Region>
  <wtg:PostalCode xmlns:wtg="https://www.wisetechglobal.com/"></wtg:PostalCode>
  <wtg:Country xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Country>
  <wtg:Residential xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Residential>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName8</wtg:CompanyName>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale0</wtg:Locale>
  <wtg:Other xmlns:wtg="https://www.wisetechglobal.com/">Other0</wtg:Other>
  <wtg:RegionName xmlns:wtg="https://www.wisetechglobal.com/">RegionName4</wtg:RegionName>
  <wtg:CountryName xmlns:wtg="https://www.wisetechglobal.com/">CountryName4</wtg:CountryName>
</wtg:Address>
```

