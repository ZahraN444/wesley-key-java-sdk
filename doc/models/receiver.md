
# Receiver

Container for the receiver address details associated with the transaction.

## Structure

`Receiver`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
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
| `Residential` | `Boolean` | Optional | Indicates whether the address is residential or commercial.<br><br>**Default**: `false` | Boolean getResidential() | setResidential(Boolean residential) |
| `Phone` | `String` | Optional | The receiver's phone number. | String getPhone() | setPhone(String phone) |
| `DepartmentName` | `String` | Optional | Name of the department that the shipment is to be delivered to. Only used for special 'In-building' deliveries. | String getDepartmentName() | setDepartmentName(String departmentName) |
| `IDNumber` | `String` | Optional | Identification number of receiver. | String getIDNumber() | setIDNumber(String iDNumber) |
| `IDType` | [`IDTypeEnum`](../../doc/models/id-type-enum.md) | Optional | ID Number Type | IDTypeEnum getIDType() | setIDType(IDTypeEnum iDType) |
| `TaxNumber` | `String` | Optional | Tax identification number of receiver. | String getTaxNumber() | setTaxNumber(String taxNumber) |
| `TaxType` | [`TaxTypeEnum`](../../doc/models/tax-type-enum.md) | Optional | Tax Number Type | TaxTypeEnum getTaxType() | setTaxType(TaxTypeEnum taxType) |

## Example (as XML)

```xml
<wtg:Receiver xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Residential xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Residential>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName8</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street6</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale0</wtg:Locale>
  <wtg:Other xmlns:wtg="https://www.wisetechglobal.com/">Other0</wtg:Other>
  <wtg:City xmlns:wtg="https://www.wisetechglobal.com/">City4</wtg:City>
</wtg:Receiver>
```

