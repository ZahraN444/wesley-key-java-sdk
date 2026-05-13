
# Billing

Container for billing details associated with the transaction.

## Structure

`Billing`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PayerType` | `Integer` | Optional | The unique numeric identifier for the type of payer.<br><br>**Default**: `0` | Integer getPayerType() | setPayerType(Integer payerType) |
| `AccountNumber` | `String` | Optional | An optional account number associated with the payer. | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `Name` | `String` | Optional | Name of the individual sending the shipment. | String getName() | setName(String name) |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Optional | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Optional | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address. | String getRegion() | setRegion(String region) |
| `RegionName` | `String` | Optional | The name of the region associated with the address, this value will be automatically added if available. | String getRegionName() | setRegionName(String regionName) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address. | String getCountry() | setCountry(String country) |
| `Phone` | `String` | Optional | The phone number associated with the address. | String getPhone() | setPhone(String phone) |
| `Email` | `String` | Optional | An email address for the individual or company. | String getEmail() | setEmail(String email) |
| `CountryName` | `String` | Optional | The name of the country associated with the address, this value will be automatically added if available. | String getCountryName() | setCountryName(String countryName) |

## Example (as XML)

```xml
<wtg:Billing xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:PayerType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PayerType>
  <wtg:AccountNumber xmlns:wtg="https://www.wisetechglobal.com/">AccountNumber8</wtg:AccountNumber>
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name6</wtg:Name>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName4</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street2</wtg:Street>
</wtg:Billing>
```

