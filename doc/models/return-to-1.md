
# Return to 1

Container for any return address assocaited with the transaction.

## Structure

`ReturnTo1`

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
| `PostalCode` | `String` | Required | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Required | The country code for the address. | String getCountry() | setCountry(String country) |
| `Phone` | `String` | Required | The phone number associated with the address. | String getPhone() | setPhone(String phone) |

## Example (as XML)

```xml
<wtg:ReturnTo xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name0</wtg:Name>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName0</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street8</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale2</wtg:Locale>
  <wtg:Other xmlns:wtg="https://www.wisetechglobal.com/">Other2</wtg:Other>
  <wtg:City xmlns:wtg="https://www.wisetechglobal.com/">City8</wtg:City>
  <wtg:Region xmlns:wtg="https://www.wisetechglobal.com/">Region0</wtg:Region>
  <wtg:PostalCode xmlns:wtg="https://www.wisetechglobal.com/">PostalCode2</wtg:PostalCode>
  <wtg:Country xmlns:wtg="https://www.wisetechglobal.com/">Country4</wtg:Country>
  <wtg:Phone xmlns:wtg="https://www.wisetechglobal.com/">Phone2</wtg:Phone>
</wtg:ReturnTo>
```

