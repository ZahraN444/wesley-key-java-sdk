
# Billing 4

Container for billing details associated with the transaction.

## Structure

`Billing4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PayerType` | `Integer` | Optional | The unique numeric identifier for the type of payer.<br><br>**Default**: `0` | Integer getPayerType() | setPayerType(Integer payerType) |
| `Name` | `String` | Optional | Name of the individual sending the shipment. | String getName() | setName(String name) |
| `AccountNumber` | `String` | Optional | An optional account number associated with the payer. | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Optional | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Optional | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address. | String getCountry() | setCountry(String country) |
| `Phone` | `String` | Optional | The phone number associated with the address. | String getPhone() | setPhone(String phone) |
| `Email` | `String` | Optional | An email address for the individual or company. | String getEmail() | setEmail(String email) |
| `ExternalSystemCode` | `String` | Optional | Bill to code for external system. | String getExternalSystemCode() | setExternalSystemCode(String externalSystemCode) |

## Example (as XML)

```xml
<wtg:Billing xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:PayerType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PayerType>
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name8</wtg:Name>
  <wtg:AccountNumber xmlns:wtg="https://www.wisetechglobal.com/">AccountNumber2</wtg:AccountNumber>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName8</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street6</wtg:Street>
</wtg:Billing>
```

