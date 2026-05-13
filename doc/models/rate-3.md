
# Rate 3

Container for an individual rate.

## Structure

`Rate3`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Status` | [`Status1`](../../doc/models/status-1.md) | Required | Container for transaction errors and warning elements. | Status1 getStatus() | setStatus(Status1 status) |
| `Carrier` | [`Carrier`](../../doc/models/carrier.md) | Optional | Container element for the carrier. | Carrier getCarrier() | setCarrier(Carrier carrier) |
| `ServiceType` | [`ServiceType`](../../doc/models/service-type.md) | Optional | Container element for the carrier service. | ServiceType getServiceType() | setServiceType(ServiceType serviceType) |
| `PackageType` | [`PackageType`](../../doc/models/package-type.md) | Optional | Container element for the carrier package type. | PackageType getPackageType() | setPackageType(PackageType packageType) |
| `Interline` | `Boolean` | Optional | Indicates that another carrier maybe be involved with part of the delivery.<br><br>**Default**: `false` | Boolean getInterline() | setInterline(Boolean interline) |
| `Shipping` | [`Shipping`](../../doc/models/shipping.md) | Optional | Container for shipping associated with the transaction. | Shipping getShipping() | setShipping(Shipping shipping) |
| `Customer` | [`Customer`](../../doc/models/customer.md) | Optional | Container for customer details. | Customer getCustomer() | setCustomer(Customer customer) |
| `BrokerReference` | `String` | Optional | Broker reference. | String getBrokerReference() | setBrokerReference(String brokerReference) |
| `CommitmentLevel` | `String` | Optional | Returned by the carrier indicating the expected delivery date and time. | String getCommitmentLevel() | setCommitmentLevel(String commitmentLevel) |
| `ServiceIsGuaranteed` | `Boolean` | Optional | Indicates a guaranteed service. | Boolean getServiceIsGuaranteed() | setServiceIsGuaranteed(Boolean serviceIsGuaranteed) |
| `DeliverAfterTime` | `String` | Optional | Identifies a delivery window. | String getDeliverAfterTime() | setDeliverAfterTime(String deliverAfterTime) |
| `RateType` | `Integer` | Optional | Numeric identifier for the rate type.<br><br>**Default**: `0` | Integer getRateType() | setRateType(Integer rateType) |
| `RateDescription` | `String` | Optional | Free form description for the rate type. | String getRateDescription() | setRateDescription(String rateDescription) |
| `RateWeight` | `Double` | Optional | The rated weight for the package.<br><br>**Default**: `0d` | Double getRateWeight() | setRateWeight(Double rateWeight) |
| `ShipDate` | `String` | Optional | Date the items where shipped. | String getShipDate() | setShipDate(String shipDate) |
| `DeliveryDate` | `String` | Optional | The requested delivery date for the shipment. | String getDeliveryDate() | setDeliveryDate(String deliveryDate) |
| `DeliveryIn` | `Integer` | Optional | Returned by the carrier indicating the number of days the shipment will take to reach its destination.<br><br>**Default**: `0` | Integer getDeliveryIn() | setDeliveryIn(Integer deliveryIn) |
| `DisplayRate` | `Boolean` | Optional | Indicates if the rate is marked for display to the user.<br><br>**Default**: `false` | Boolean getDisplayRate() | setDisplayRate(Boolean displayRate) |
| `UpdateRate` | `Boolean` | Optional | Indicates if the rate is used during updates back to customer host systems.<br><br>**Default**: `false` | Boolean getUpdateRate() | setUpdateRate(Boolean updateRate) |
| `Zone` | `String` | Optional | The zone assosicated with the rate. | String getZone() | setZone(String zone) |
| `QuoteID` | `String` | Optional | The unique quote identifier for freight based transactions. | String getQuoteID() | setQuoteID(String quoteID) |
| `OptionID` | `String` | Optional | The unique option identifier for freight based transactions. | String getOptionID() | setOptionID(String optionID) |
| `ChargeGroups` | [`ChargeGroups1`](../../doc/models/charge-groups-1.md) | Optional | Container for all charge groups associated with the transaction. | ChargeGroups1 getChargeGroups() | setChargeGroups(ChargeGroups1 chargeGroups) |
| `Packages` | [`Packages4`](../../doc/models/packages-4.md) | Optional | Container for all packages relating to the specific rate. | Packages4 getPackages() | setPackages(Packages4 packages) |

## Example (as XML)

```xml
<wtg:Rate xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Status>
  <wtg:Interline xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Interline>
  <wtg:RateType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:RateType>
  <wtg:RateWeight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:RateWeight>
  <wtg:DeliveryIn xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:DeliveryIn>
  <wtg:DisplayRate xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DisplayRate>
  <wtg:UpdateRate xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:UpdateRate>
  <wtg:Carrier xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Carrier>
  <wtg:ServiceType xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ServiceType>
  <wtg:PackageType xmlns:wtg="https://www.wisetechglobal.com/"></wtg:PackageType>
  <wtg:Shipping xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Shipping>
</wtg:Rate>
```

