
# Sender 1

Container to allow the customization of the sender address details associated with the transaction.

## Structure

`Sender1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `SentBy` | `String` | Optional | Name of the individual sending the shipment. | String getSentBy() | setSentBy(String sentBy) |
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
| `JobTitle` | `String` | Optional | Job title of the individual sending the shipment. | String getJobTitle() | setJobTitle(String jobTitle) |
| `DepartmentName` | `String` | Optional | Department name of the individual sending the shipment. | String getDepartmentName() | setDepartmentName(String departmentName) |
| `LocationDescription` | `String` | Optional | Location description of the shipper. | String getLocationDescription() | setLocationDescription(String locationDescription) |
| `LocationTimeZone` | `String` | Optional | Carrier specific data indicating time zone of sender's location. | String getLocationTimeZone() | setLocationTimeZone(String locationTimeZone) |
| `Residential` | `Boolean` | Optional | Indicates whether the address is residential or commercial.<br><br>**Default**: `false` | Boolean getResidential() | setResidential(Boolean residential) |
| `OverrideType` | [`OverrideTypeEnum`](../../doc/models/override-type-enum.md) | Optional | Indicates what type of override is being used for sender information.  You can override all information, only the nonessential information (e.g. phone, email) or do no overriding.  If you choose none, then all sender information is read from the configuration. | OverrideTypeEnum getOverrideType() | setOverrideType(OverrideTypeEnum overrideType) |

## Example (as XML)

```xml
<wtg:Sender xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Residential xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Residential>
  <wtg:SentBy xmlns:wtg="https://www.wisetechglobal.com/">SentBy6</wtg:SentBy>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName0</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street8</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale2</wtg:Locale>
  <wtg:Other xmlns:wtg="https://www.wisetechglobal.com/">Other2</wtg:Other>
</wtg:Sender>
```

