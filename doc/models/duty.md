
# Duty

Container for duty details assocaited with the transaction.

## Structure

`Duty`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PayerType` | `Integer` | Optional | Type of payer the shipment's duties and taxes are to be billed to.  Defaults to sender if not submitted.<br><br>**Default**: `0` | Integer getPayerType() | setPayerType(Integer payerType) |
| `AccountNumber` | `String` | Optional | Account number the shipment's duties and taxes are to be billed to.  Defaults to sender's account number if not submitted. | String getAccountNumber() | setAccountNumber(String accountNumber) |
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
| `Contact` | `String` | Optional | Name of the person the shipment's duties and taxes are to be billed to. | String getContact() | setContact(String contact) |

## Example (as XML)

```xml
<wtg:Duty xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:PayerType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PayerType>
  <wtg:AccountNumber xmlns:wtg="https://www.wisetechglobal.com/">AccountNumber2</wtg:AccountNumber>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName8</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street6</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale0</wtg:Locale>
</wtg:Duty>
```

