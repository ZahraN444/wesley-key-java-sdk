
# Broker 1

Container for broker details.

## Structure

`Broker1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `BrokerID` | `Integer` | Optional | Export broker who will handle the shipment.<br><br>**Default**: `0` | Integer getBrokerID() | setBrokerID(Integer brokerID) |
| `BrokerType` | [`BrokerTypeEnum`](../../doc/models/broker-type-enum.md) | Optional | Export broker who will handle the shipment. | BrokerTypeEnum getBrokerType() | setBrokerType(BrokerTypeEnum brokerType) |
| `Contact` | `String` | Optional | Broker contact who will handle the shipment. | String getContact() | setContact(String contact) |
| `Phone` | `String` | Optional | Export broker phone number. | String getPhone() | setPhone(String phone) |
| `EMail` | `String` | Optional | Export broker email address. | String getEMail() | setEMail(String eMail) |
| `Fax` | `String` | Optional | Export broker fax number. | String getFax() | setFax(String fax) |
| `AccountNumber` | `String` | Optional | Export broker account number. | String getAccountNumber() | setAccountNumber(String accountNumber) |
| `Organization` | `String` | Optional | Export broker organization name. | String getOrganization() | setOrganization(String organization) |
| `Street` | `String` | Optional | Export broker address street. | String getStreet() | setStreet(String street) |
| `Locale` | `String` | Optional | Export broker address locale. | String getLocale() | setLocale(String locale) |
| `City` | `String` | Optional | Export broker address city name. | String getCity() | setCity(String city) |
| `Region` | `String` | Optional | Export broker address region. | String getRegion() | setRegion(String region) |
| `PostalCode` | `String` | Optional | Export broker address postal code. | String getPostalCode() | setPostalCode(String postalCode) |
| `Country` | `String` | Optional | Export broker address country code. | String getCountry() | setCountry(String country) |
| `IdentificationNumber` | `String` | Optional | The Tax Identification Number of the individual acting as  broker. | String getIdentificationNumber() | setIdentificationNumber(String identificationNumber) |
| `IdentificationNumberType` | [`IdentificationNumberTypeEnum`](../../doc/models/identification-number-type-enum.md) | Optional | The Tax Identification Number Type of the individual acting as broker. | IdentificationNumberTypeEnum getIdentificationNumberType() | setIdentificationNumberType(IdentificationNumberTypeEnum identificationNumberType) |

## Example (as XML)

```xml
<wtg:Broker xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:BrokerID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:BrokerID>
  <wtg:BrokerType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:BrokerType>
  <wtg:Contact xmlns:wtg="https://www.wisetechglobal.com/">Contact6</wtg:Contact>
  <wtg:Phone xmlns:wtg="https://www.wisetechglobal.com/">Phone6</wtg:Phone>
  <wtg:EMail xmlns:wtg="https://www.wisetechglobal.com/">EMail4</wtg:EMail>
</wtg:Broker>
```

