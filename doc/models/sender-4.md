
# Sender 4

Container to allow the customization of the sender address details associated with the transaction.

## Structure

`Sender4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `SentBy` | `String` | Optional | The name of the sender. | String getSentBy() | setSentBy(String sentBy) |
| `Phone` | `String` | Optional | The phone number associated with the address. | String getPhone() | setPhone(String phone) |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Optional | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Optional | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address. | String getCountry() | setCountry(String country) |
| `Email` | `String` | Optional | The email address for the sender of the package. | String getEmail() | setEmail(String email) |
| `DepartmentName` | `String` | Optional | The department for the sender of the package. | String getDepartmentName() | setDepartmentName(String departmentName) |
| `LocationDescription` | `String` | Optional | The description of the location associated with the address. | String getLocationDescription() | setLocationDescription(String locationDescription) |

## Example (as XML)

```xml
<wtg:Sender xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:SentBy xmlns:wtg="https://www.wisetechglobal.com/">SentBy8</wtg:SentBy>
  <wtg:Phone xmlns:wtg="https://www.wisetechglobal.com/">Phone4</wtg:Phone>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName2</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street0</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale4</wtg:Locale>
</wtg:Sender>
```

