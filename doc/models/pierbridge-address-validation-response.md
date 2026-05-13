
# Pierbridge Address Validation Response

Indicates the status of an AddressValidation request.

## Structure

`PierbridgeAddressValidationResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TransactionIdentifier` | `String` | Optional | The unique identifier for the transaction given in the request. | String getTransactionIdentifier() | setTransactionIdentifier(String transactionIdentifier) |
| `ControlIdentifier` | `String` | Optional | The control reference for the transaction given in the request. | String getControlIdentifier() | setControlIdentifier(String controlIdentifier) |
| `Status` | [`Status`](../../doc/models/status.md) | Required | Container for transaction errors and warning elements. | Status getStatus() | setStatus(Status status) |
| `OriginalAddressValidated` | `Boolean` | Optional | Indicates if the address given in the request was validated successfully.<br><br>**Default**: `false` | Boolean getOriginalAddressValidated() | setOriginalAddressValidated(Boolean originalAddressValidated) |
| `OriginalAddressResidential` | `Boolean` | Optional | Indicates if the address given in the request was marked as being residential.<br><br>**Default**: `false` | Boolean getOriginalAddressResidential() | setOriginalAddressResidential(Boolean originalAddressResidential) |
| `AlternateAddresses` | [`AlternateAddresses`](../../doc/models/alternate-addresses.md) | Optional | Container for alternative addresses for the address given in the request. | AlternateAddresses getAlternateAddresses() | setAlternateAddresses(AlternateAddresses alternateAddresses) |
| `Carrier` | `String` | Optional | Numeric identifier for the carrier. | String getCarrier() | setCarrier(String carrier) |
| `CarrierName` | `String` | Optional | The name for the carrier. | String getCarrierName() | setCarrierName(String carrierName) |
| `CarrierScac` | `String` | Optional | The NMFTA (National Motor Freight Traffic Association) Standard Carrier Alpha Code of the carrier. | String getCarrierScac() | setCarrierScac(String carrierScac) |
| `Processing` | [`Processing`](../../doc/models/processing.md) | Required | Container element for transaction processing statistics. | Processing getProcessing() | setProcessing(Processing processing) |

## Example (as XML)

```xml
<wtg:PierbridgeAddressValidationResponse xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Status>
  <wtg:OriginalAddressValidated xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OriginalAddressValidated>
  <wtg:OriginalAddressResidential xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OriginalAddressResidential>
  <wtg:Processing xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Processing>
  <wtg:TransactionIdentifier xmlns:wtg="https://www.wisetechglobal.com/">TransactionIdentifier2</wtg:TransactionIdentifier>
  <wtg:ControlIdentifier xmlns:wtg="https://www.wisetechglobal.com/">ControlIdentifier2</wtg:ControlIdentifier>
  <wtg:AlternateAddresses xmlns:wtg="https://www.wisetechglobal.com/"></wtg:AlternateAddresses>
</wtg:PierbridgeAddressValidationResponse>
```

