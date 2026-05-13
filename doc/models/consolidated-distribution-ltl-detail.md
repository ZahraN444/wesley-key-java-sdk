
# Consolidated Distribution Ltl Detail

Container for details for origin-country LTL services performed by carrier

## Structure

`ConsolidatedDistributionLtlDetail`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PaymentType` | `Integer` | Optional | The payment type of the payor responsible for paying for the origin-country LTL services performed by carrier | Integer getPaymentType() | setPaymentType(Integer paymentType) |
| `LtlScacCode` | `String` | Optional | An optional scac code associated with the origin-country LTL services performed by carrier | String getLtlScacCode() | setLtlScacCode(String ltlScacCode) |
| `AccountNumber` | `String` | Optional | An account number of the company responsioble for paying for the origin-country LTL services performed by carrier | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `Name` | `String` | Optional | Name of the individual responsible for paying for the origin-country LTL services performed by carrier. | String getName() | setName(String name) |
| `CompanyName` | `String` | Optional | Name of the company responsible for paying for the origin-country LTL services performed by carrier. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Optional | First line of the address for the person/company responsible for paying for the origin-country LTL services performed by carrier. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address for the person/company responsible for paying for the origin-country LTL services performed by carrier. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Optional | City of the address for the person/company responsible for paying for the origin-country LTL services performed by carrier. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address for the person/company responsible for paying for the origin-country LTL services performed by carrier. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address for the person/company responsible for paying for the origin-country LTL services performed by carrier. | String getCountry() | setCountry(String country) |
| `Phone` | `String` | Optional | The phone number associated with the address for the person/company responsible for paying for the origin-country LTL services performed by carrier. | String getPhone() | setPhone(String phone) |
| `Email` | `String` | Optional | The email associated with the address for the person/company responsible for paying for the origin-country LTL services performed by carrier. | String getEmail() | setEmail(String email) |

## Example (as XML)

```xml
<wtg:ConsolidatedDistributionLtlDetail xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:PaymentType xmlns:wtg="https://www.wisetechglobal.com/">78</wtg:PaymentType>
  <wtg:LtlScacCode xmlns:wtg="https://www.wisetechglobal.com/">LtlScacCode6</wtg:LtlScacCode>
  <wtg:AccountNumber xmlns:wtg="https://www.wisetechglobal.com/">AccountNumber2</wtg:AccountNumber>
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name2</wtg:Name>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName8</wtg:CompanyName>
</wtg:ConsolidatedDistributionLtlDetail>
```

