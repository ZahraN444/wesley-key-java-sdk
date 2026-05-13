
# Receiver 4

Container for the receiver address details associated with the transaction.

## Structure

`Receiver4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AccountNumber` | `String` | Optional | The receivers account number. | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `CompanyName` | `String` | Optional | The company name associated with the address. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Required | First line of the address. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address. | String getLocale() | setLocale(String locale) |
| `Other` | `String` | Optional | Third line of the address. | String getOther() | setOther(String other) |
| `City` | `String` | Required | City of the address. | String getCity() | setCity(String city) |
| `Region` | `String` | Required | The state or region of the address. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Required | The postal code or zip associated with the address. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Required | The country code for the address. | String getCountry() | setCountry(String country) |
| `Residential` | `Boolean` | Optional | Indicates whether the address is residential or commercial.<br><br>**Default**: `false` | Boolean getResidential() | setResidential(Boolean residential) |
| `Modified` | `Boolean` | Optional | Indicates whether the address to be shipped to has been modified.  Defaults to not modified if not submitted.<br><br>**Default**: `false` | Boolean getModified() | setModified(Boolean modified) |
| `ExternalReceiverID` | `String` | Optional | Identifier value used to identify the receiver in an external system. | String getExternalReceiverID() | setExternalReceiverID(String externalReceiverID) |
| `DepartmentName` | `String` | Optional | Name of the department that the shipment is to be delivered to. Only used for special 'In-building' deliveries. | String getDepartmentName() | setDepartmentName(String departmentName) |
| `IDNumber` | `String` | Optional | Identification number of receiver. | String getIDNumber() | setIDNumber(String iDNumber) |
| `IDType` | [`IDTypeEnum`](../../doc/models/id-type-enum.md) | Optional | ID Number Type | IDTypeEnum getIDType() | setIDType(IDTypeEnum iDType) |
| `TaxNumber` | `String` | Optional | Tax identification number of receiver. | String getTaxNumber() | setTaxNumber(String taxNumber) |
| `TaxType` | [`TaxTypeEnum`](../../doc/models/tax-type-enum.md) | Optional | Tax Number Type | TaxTypeEnum getTaxType() | setTaxType(TaxTypeEnum taxType) |

## Example (as XML)

```xml
<wtg:Receiver xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Street>
  <wtg:City xmlns:wtg="https://www.wisetechglobal.com/"></wtg:City>
  <wtg:Region xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Region>
  <wtg:PostalCode xmlns:wtg="https://www.wisetechglobal.com/"></wtg:PostalCode>
  <wtg:Country xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Country>
  <wtg:Residential xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Residential>
  <wtg:Modified xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Modified>
  <wtg:AccountNumber xmlns:wtg="https://www.wisetechglobal.com/">AccountNumber2</wtg:AccountNumber>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName8</wtg:CompanyName>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale0</wtg:Locale>
  <wtg:Other xmlns:wtg="https://www.wisetechglobal.com/">Other0</wtg:Other>
</wtg:Receiver>
```

