
# Holder

Container for the holding location of the package.

## Structure

`Holder`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `HoldLocationID` | `String` | Optional | Carrier identifier for the hold location. | String getHoldLocationID() | setHoldLocationID(String holdLocationID) |
| `Name` | `String` | Optional | Name of the individual who is to hold the package for collection. | String getName() | setName(String name) |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Optional | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Optional | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address. | String getCountry() | setCountry(String country) |
| `Phone` | `String` | Optional | The phone number associated with the address. | String getPhone() | setPhone(String phone) |
| `Type` | `String` | Optional | The holder type associated with the address. | String getType() | setType(String type) |

## Example (as XML)

```xml
<wtg:Holder xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:HoldLocationID xmlns:wtg="https://www.wisetechglobal.com/">HoldLocationID4</wtg:HoldLocationID>
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name4</wtg:Name>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName4</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street2</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale6</wtg:Locale>
</wtg:Holder>
```

