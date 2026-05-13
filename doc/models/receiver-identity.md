
# Receiver Identity

Container element for receiver identification details.

## Structure

`ReceiverIdentity`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DocumentIDNumber` | `String` | Optional | The ID number of the document (e.g. passport, ID card) used to identify the received. Used for specific 'ID check' delivery methods. | String getDocumentIDNumber() | setDocumentIDNumber(String documentIDNumber) |
| `DocumentType` | `String` | Optional | The type of document used to identify the received. Used for specific 'ID check' delivery methods. | String getDocumentType() | setDocumentType(String documentType) |
| `DateOfBirth` | `String` | Optional | Date of birth of the receiver. | String getDateOfBirth() | setDateOfBirth(String dateOfBirth) |
| `FirstName` | `String` | Optional | The first name individual associated with the address. | String getFirstName() | setFirstName(String firstName) |
| `LastName` | `String` | Optional | Last name of the receiver. Defaults to regular receiver name if left blank. | String getLastName() | setLastName(String lastName) |

## Example (as XML)

```xml
<wtg:ReceiverIdentity xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:DocumentIDNumber xmlns:wtg="https://www.wisetechglobal.com/">DocumentIDNumber6</wtg:DocumentIDNumber>
  <wtg:DocumentType xmlns:wtg="https://www.wisetechglobal.com/">DocumentType2</wtg:DocumentType>
  <wtg:DateOfBirth xmlns:wtg="https://www.wisetechglobal.com/">DateOfBirth6</wtg:DateOfBirth>
  <wtg:FirstName xmlns:wtg="https://www.wisetechglobal.com/">FirstName2</wtg:FirstName>
  <wtg:LastName xmlns:wtg="https://www.wisetechglobal.com/">LastName8</wtg:LastName>
</wtg:ReceiverIdentity>
```

