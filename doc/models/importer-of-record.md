
# Importer of Record

Container for importer of record details.

## Structure

`ImporterOfRecord`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AccountNumber` | `String` | Optional | An optional account number associated with the importer | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Name` | `String` | Optional | Name of the contact at the importer. | String getName() | setName(String name) |
| `Street` | `String` | Optional | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Other of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Optional | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address. | String getCountry() | setCountry(String country) |
| `Phone` | `String` | Optional | The phone number associated with the address. | String getPhone() | setPhone(String phone) |
| `IdentificationNumber` | `String` | Optional | Account number of the importer. | String getIdentificationNumber() | setIdentificationNumber(String identificationNumber) |
| `ImporterOfRecordTaxID` | `String` | Optional | Tax Identifier of the importer. | String getImporterOfRecordTaxID() | setImporterOfRecordTaxID(String importerOfRecordTaxID) |
| `ImporterOfRecordTaxIDType` | [`ImporterOfRecordTaxIDTypeEnum`](../../doc/models/importer-of-record-tax-id-type-enum.md) | Optional | The Tax Identification Number Type of the importer. | ImporterOfRecordTaxIDTypeEnum getImporterOfRecordTaxIDType() | setImporterOfRecordTaxIDType(ImporterOfRecordTaxIDTypeEnum importerOfRecordTaxIDType) |
| `Email` | `String` | Optional | An email address for the individual or company. | String getEmail() | setEmail(String email) |

## Example (as XML)

```xml
<wtg:ImporterOfRecord xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:AccountNumber xmlns:wtg="https://www.wisetechglobal.com/">AccountNumber8</wtg:AccountNumber>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName4</wtg:CompanyName>
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name4</wtg:Name>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street2</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale6</wtg:Locale>
</wtg:ImporterOfRecord>
```

