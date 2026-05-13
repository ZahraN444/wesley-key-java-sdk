
# Return To

Container for any return address assocaited with the transaction.

## Structure

`ReturnTo`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Name` | `String` | Required | Name of the individual the shipment is to be returned to. | String getName() | setName(String name) |
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
| `Phone` | `String` | Required | The phone number associated with the address. | String getPhone() | setPhone(String phone) |

## Example (as XML)

```xml
<wtg:ReturnTo xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name2</wtg:Name>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName2</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street0</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale4</wtg:Locale>
  <wtg:Other xmlns:wtg="https://www.wisetechglobal.com/">Other4</wtg:Other>
  <wtg:City xmlns:wtg="https://www.wisetechglobal.com/">City0</wtg:City>
  <wtg:Region xmlns:wtg="https://www.wisetechglobal.com/">Region2</wtg:Region>
  <wtg:RegionName xmlns:wtg="https://www.wisetechglobal.com/">RegionName2</wtg:RegionName>
  <wtg:PostalCode xmlns:wtg="https://www.wisetechglobal.com/">PostalCode4</wtg:PostalCode>
  <wtg:Country xmlns:wtg="https://www.wisetechglobal.com/">Country6</wtg:Country>
  <wtg:CountryName xmlns:wtg="https://www.wisetechglobal.com/">CountryName8</wtg:CountryName>
  <wtg:Phone xmlns:wtg="https://www.wisetechglobal.com/">Phone4</wtg:Phone>
</wtg:ReturnTo>
```

