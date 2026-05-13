
# Billing 3

Container for billing details associated with the transaction.

## Structure

`Billing3`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PayerType` | `Integer` | Optional | The unique numeric identifier for the type of payer.<br><br>**Default**: `0` | Integer getPayerType() | setPayerType(Integer payerType) |
| `AccountNumber` | `String` | Optional | An optional account number associated with the payer. | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Optional | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Optional | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address. | String getCountry() | setCountry(String country) |

## Example (as XML)

```xml
<wtg:Billing xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:PayerType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PayerType>
  <wtg:AccountNumber xmlns:wtg="https://www.wisetechglobal.com/">AccountNumber0</wtg:AccountNumber>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName6</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street4</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale8</wtg:Locale>
</wtg:Billing>
```

