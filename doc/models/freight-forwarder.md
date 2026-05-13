
# Freight Forwarder

Container to allow the customization of the freight forwarder address details associated with the transaction.

## Structure

`FreightForwarder`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Name` | `String` | Optional | Name of the individual acting as an agent for the exporter in moving cargo to an overseas destination. | String getName() | setName(String name) |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Optional | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Optional | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address. | String getRegion() | setRegion(String region) |
| `RegionName` | `String` | Optional | The name of the region associated with the address, this value will be automatically added if available. | String getRegionName() | setRegionName(String regionName) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address. | String getCountry() | setCountry(String country) |
| `CountryName` | `String` | Optional | The name of the country associated with the address, this value will be automatically added if available. | String getCountryName() | setCountryName(String countryName) |
| `Phone` | `String` | Optional | The phone number associated with the address. | String getPhone() | setPhone(String phone) |
| `IdentificationNumber` | `String` | Optional | Identification number (e.g. EIN, SSN, DUNS) of the individual acting as an agent for the exporter in moving cargo to an overseas destination. | String getIdentificationNumber() | setIdentificationNumber(String identificationNumber) |
| `IdentificationNumberType` | `Integer` | Optional | Type of the identification number (e.g. EIN, SSN, DUNS) of the individual acting as an agent for the exporter in moving cargo to an overseas destination.<br><br>**Default**: `0` | Integer getIdentificationNumberType() | setIdentificationNumberType(Integer identificationNumberType) |

## Example (as XML)

```xml
<wtg:FreightForwarder xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:IdentificationNumberType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:IdentificationNumberType>
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name2</wtg:Name>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName2</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street0</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale4</wtg:Locale>
  <wtg:Other xmlns:wtg="https://www.wisetechglobal.com/">Other4</wtg:Other>
</wtg:FreightForwarder>
```

