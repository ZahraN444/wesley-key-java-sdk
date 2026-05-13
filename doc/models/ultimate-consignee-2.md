
# Ultimate Consignee 2

Container to allow the customization of the ultimate consignee address details associated with the transaction.

## Structure

`UltimateConsignee2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AccountNumber` | `String` | Optional | Account number of individual actually receiving the merchandise. | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `Name` | `String` | Optional | Name of the individual actually receiving the merchandise. | String getName() | setName(String name) |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Optional | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Optional | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address. | String getCountry() | setCountry(String country) |
| `Phone` | `String` | Optional | The phone number associated with the address. | String getPhone() | setPhone(String phone) |
| `Email` | `String` | Optional | Email address. | String getEmail() | setEmail(String email) |

## Example (as XML)

```xml
<wtg:UltimateConsignee xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:AccountNumber xmlns:wtg="https://www.wisetechglobal.com/">AccountNumber6</wtg:AccountNumber>
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name2</wtg:Name>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName2</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street0</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale4</wtg:Locale>
</wtg:UltimateConsignee>
```

