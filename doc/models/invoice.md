
# Invoice

Container for address details where the shipment costs should be invoiced.

## Structure

`Invoice`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Optional | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Optional | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address. | String getCountry() | setCountry(String country) |
| `TaxIdentifier` | `String` | Optional | Tax identifier the shipment is to be invoiced to. | String getTaxIdentifier() | setTaxIdentifier(String taxIdentifier) |
| `Number` | `String` | Optional | Invoice number assigned to shipment. | String getNumber() | setNumber(String number) |
| `ContactName` | `String` | Optional | Name of the individual associated with the address. | String getContactName() | setContactName(String contactName) |
| `Phone` | `String` | Optional | The phone number associated with the address. | String getPhone() | setPhone(String phone) |
| `Email` | `String` | Optional | An email address for the individual or company. | String getEmail() | setEmail(String email) |

## Example (as XML)

```xml
<wtg:Invoice xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName0</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street8</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale2</wtg:Locale>
  <wtg:Other xmlns:wtg="https://www.wisetechglobal.com/">Other2</wtg:Other>
  <wtg:City xmlns:wtg="https://www.wisetechglobal.com/">City8</wtg:City>
</wtg:Invoice>
```

