
# Receiver 5

Container for the receiver address details associated with the transaction.

## Structure

`Receiver5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
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
| `Residential` | `Boolean` | Optional | Indicates whether the address is residential or commercial.<br><br>**Default**: `false` | Boolean getResidential() | setResidential(Boolean residential) |
| `Modified` | `Boolean` | Optional | Indicates whether the address has been modified as provided in the request.<br><br>**Default**: `false` | Boolean getModified() | setModified(Boolean modified) |
| `ExternalReceiverID` | `String` | Optional | Identifier for the receiver which has been assigned by an external system. | String getExternalReceiverID() | setExternalReceiverID(String externalReceiverID) |
| `DepartmentName` | `String` | Optional | Department name of the individual sending the shipment. | String getDepartmentName() | setDepartmentName(String departmentName) |
| `Phone` | `String` | Optional | Recipient's phone number. | String getPhone() | setPhone(String phone) |

## Example (as XML)

```xml
<wtg:Receiver xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Residential xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Residential>
  <wtg:Modified xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Modified>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName4</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street2</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale6</wtg:Locale>
  <wtg:Other xmlns:wtg="https://www.wisetechglobal.com/">Other6</wtg:Other>
  <wtg:City xmlns:wtg="https://www.wisetechglobal.com/">City2</wtg:City>
</wtg:Receiver>
```

