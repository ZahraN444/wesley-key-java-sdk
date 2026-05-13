
# Label Origin Address

Container to allow the customization of the sender address details associated with the label

## Structure

`LabelOriginAddress`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Name` | `String` | Optional | Name of the individual sending the shipment to show on the label. | String getName() | setName(String name) |
| `CompanyName` | `String` | Optional | The company name associated with the address to show on the label. | String getCompanyName() | setCompanyName(String companyName) |
| `Street` | `String` | Optional | First line of the address to show on the label. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Second line of the address to show on the label. | String getLocale() | setLocale(String locale) |
| `City` | `String` | Optional | City of the address to show on the label. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | The state or region of the address to show on the label. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Optional | The postal code or zip associated with the address to show on the label. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | The country code for the address to show on the label. | String getCountry() | setCountry(String country) |
| `Phone` | `String` | Optional | The phone number associated with the address to show on the label. | String getPhone() | setPhone(String phone) |
| `Email` | `String` | Optional | An email address for the individual or company to show on the label. | String getEmail() | setEmail(String email) |
| `Residential` | `Boolean` | Optional | Indicates whether the address is residential or commercial.<br><br>**Default**: `false` | Boolean getResidential() | setResidential(Boolean residential) |

## Example (as XML)

```xml
<wtg:LabelOriginAddress xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Residential xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Residential>
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name4</wtg:Name>
  <wtg:CompanyName xmlns:wtg="https://www.wisetechglobal.com/">CompanyName4</wtg:CompanyName>
  <wtg:Street xmlns:wtg="https://www.wisetechglobal.com/">Street2</wtg:Street>
  <wtg:Locale xmlns:wtg="https://www.wisetechglobal.com/">Locale6</wtg:Locale>
  <wtg:City xmlns:wtg="https://www.wisetechglobal.com/">City8</wtg:City>
</wtg:LabelOriginAddress>
```

