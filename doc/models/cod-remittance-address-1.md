
# COD Remittance Address 1

Container for the COD remittance address details.

## Structure

`CODRemittanceAddress1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Name` | `String` | Optional | Name of the individual the COD Remittance should be sent to. | String getName() | setName(String name) |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Optional | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Optional | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address. | String getCountry() | setCountry(String country) |
| `Phone` | `String` | Optional | The phone number associated with the address. | String getPhone() | setPhone(String phone) |
| `DepartmentName` | `String` | Optional | Name of the department associated with the address. | String getDepartmentName() | setDepartmentName(String departmentName) |
| `IdentificationNumber` | `String` | Optional | The Tax Identification Number of the individual the COD Remittance should be sent to. | String getIdentificationNumber() | setIdentificationNumber(String identificationNumber) |
| `IdentificationNumberType` | [`IdentificationNumberTypeEnum`](../../doc/models/identification-number-type-enum.md) | Optional | The Tax Identification Number Type of the individual the COD Remittance should be sent to. | IdentificationNumberTypeEnum getIdentificationNumberType() | setIdentificationNumberType(IdentificationNumberTypeEnum identificationNumberType) |
| `AccountNumber` | `String` | Optional | Account number COD Remittance should be sent to. | String getAccountNumber() | setAccountNumber(String accountNumber) |

## Example (as XML)

```xml
<wtg:CODRemittanceAddress xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name6</wtg:Name>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName6</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street4</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale8</wtg:Locale>
  <wtg:Other xmlns:wtg="https://www.wisetechglobal.com/">Other8</wtg:Other>
</wtg:CODRemittanceAddress>
```

