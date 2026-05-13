
# Holder 3

Container for the holding location of the package.

## Structure

`Holder3`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `HoldLocationID` | `String` | Optional | Carrier identifier for the hold location. | String getHoldLocationID() | setHoldLocationID(String holdLocationID) |
| `Name` | `String` | Required | Name of the individual who is to hold the package for collection. | String getName() | setName(String name) |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Required | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Required | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Required | The state or region of the address. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Required | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Required | The country code for the address. | String getCountry() | setCountry(String country) |
| `Phone` | `String` | Required | The phone number associated with the address. | String getPhone() | setPhone(String phone) |

## Example (as XML)

```xml
<wtg:Holder xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:HoldLocationID xmlns:wtg="https://www.wisetechglobal.com/">HoldLocationID2</wtg:HoldLocationID>
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name8</wtg:Name>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName8</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street6</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale0</wtg:Locale>
  <wtg:Other xmlns:wtg="https://www.wisetechglobal.com/">Other0</wtg:Other>
  <wtg:City xmlns:wtg="https://www.wisetechglobal.com/">City4</wtg:City>
  <wtg:Region xmlns:wtg="https://www.wisetechglobal.com/">Region8</wtg:Region>
  <wtg:PostalCode xmlns:wtg="https://www.wisetechglobal.com/">PostalCode0</wtg:PostalCode>
  <wtg:Country xmlns:wtg="https://www.wisetechglobal.com/">Country2</wtg:Country>
  <wtg:Phone xmlns:wtg="https://www.wisetechglobal.com/">Phone0</wtg:Phone>
</wtg:Holder>
```

