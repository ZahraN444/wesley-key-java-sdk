
# Pierbridge Rate Shop Response

Contains the results following a RateShop request.

## Structure

`PierbridgeRateShopResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Status` | [`Status`](../../doc/models/status.md) | Required | Container for transaction errors and warning elements. | Status getStatus() | setStatus(Status status) |
| `TransactionIdentifier` | `String` | Optional | The unique identifier for the transaction given in the request. | String getTransactionIdentifier() | setTransactionIdentifier(String transactionIdentifier) |
| `ControlIdentifier` | `String` | Optional | The control reference for the transaction given in the request. | String getControlIdentifier() | setControlIdentifier(String controlIdentifier) |
| `Rates` | [`Rates3`](../../doc/models/rates-3.md) | Optional | Container all rates associated with the transaction. | Rates3 getRates() | setRates(Rates3 rates) |
| `Carrier` | `String` | Optional | Numeric identifier for the carrier. | String getCarrier() | setCarrier(String carrier) |
| `CarrierName` | `String` | Optional | The name for the carrier. | String getCarrierName() | setCarrierName(String carrierName) |
| `CarrierScac` | `String` | Optional | The NMFTA (National Motor Freight Traffic Association) Standard Carrier Alpha Code of the carrier. | String getCarrierScac() | setCarrierScac(String carrierScac) |
| `ServiceType` | `String` | Optional | Numeric identifier for the carrier service assocaited with the transaction. | String getServiceType() | setServiceType(String serviceType) |
| `ServiceTypeName` | `String` | Optional | Description of the service used for the transaction. | String getServiceTypeName() | setServiceTypeName(String serviceTypeName) |
| `ServiceIsGuaranteed` | `Boolean` | Optional | Indicates if the carrier service has a guaranteed delivery window.<br><br>**Default**: `false` | Boolean getServiceIsGuaranteed() | setServiceIsGuaranteed(Boolean serviceIsGuaranteed) |
| `DayOfWeek` | `String` | Optional | The description for the date of the shipment associated with the transaction. | String getDayOfWeek() | setDayOfWeek(String dayOfWeek) |
| `RequiredDate` | `String` | Optional | Date that the shipment is required to arrive at the receiver. | String getRequiredDate() | setRequiredDate(String requiredDate) |
| `Weight` | `Double` | Optional | Total weight of the shipment.<br><br>**Default**: `0d` | Double getWeight() | setWeight(Double weight) |
| `Receiver` | [`Receiver3`](../../doc/models/receiver-3.md) | Optional | Container for the receiver address details associated with the transaction. | Receiver3 getReceiver() | setReceiver(Receiver3 receiver) |
| `RateGroup` | `String` | Optional | Rate group name used within the transaction. | String getRateGroup() | setRateGroup(String rateGroup) |
| `FilterRateShopResult` | `String` | Optional | Indicates what rates should be returned back to the client i.e. only successful rates, success and partial failures or all rates.<br><br>**Default**: `"SuccessOnly"` | String getFilterRateShopResult() | setFilterRateShopResult(String filterRateShopResult) |
| `FreightPackages` | [`FreightPackages`](../../doc/models/freight-packages.md) | Optional | Container for all packages associated with the transaction. | FreightPackages getFreightPackages() | setFreightPackages(FreightPackages freightPackages) |
| `Packages` | [`Packages5`](../../doc/models/packages-5.md) | Optional | Container for all packages associated with the transaction. | Packages5 getPackages() | setPackages(Packages5 packages) |
| `Localization` | [`Localization1`](../../doc/models/localization-1.md) | Optional | Container for localization information. | Localization1 getLocalization() | setLocalization(Localization1 localization) |
| `Processing` | [`Processing`](../../doc/models/processing.md) | Required | Container element for transaction processing statistics. | Processing getProcessing() | setProcessing(Processing processing) |

## Example (as XML)

```xml
<wtg:PierbridgeRateShopResponse xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Status>
  <wtg:ServiceIsGuaranteed xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ServiceIsGuaranteed>
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Weight>
  <wtg:FilterRateShopResult xmlns:wtg="https://www.wisetechglobal.com/">SuccessOnly</wtg:FilterRateShopResult>
  <wtg:Processing xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Processing>
  <wtg:TransactionIdentifier xmlns:wtg="https://www.wisetechglobal.com/">TransactionIdentifier2</wtg:TransactionIdentifier>
  <wtg:ControlIdentifier xmlns:wtg="https://www.wisetechglobal.com/">ControlIdentifier2</wtg:ControlIdentifier>
  <wtg:Rates xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Rates>
  <wtg:Carrier xmlns:wtg="https://www.wisetechglobal.com/">Carrier0</wtg:Carrier>
  <wtg:CarrierName xmlns:wtg="https://www.wisetechglobal.com/">CarrierName8</wtg:CarrierName>
</wtg:PierbridgeRateShopResponse>
```

