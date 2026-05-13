
# Rate 9

Container for an individual rate.

## Structure

`Rate9`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RateType` | `Integer` | Optional | Numeric identifier for the rate type. | Integer getRateType() | setRateType(Integer rateType) |
| `RateDescription` | `String` | Optional | Free form description for the rate type. | String getRateDescription() | setRateDescription(String rateDescription) |
| `RateWeight` | `Double` | Optional | The rated weight for the package.<br><br>**Default**: `0d` | Double getRateWeight() | setRateWeight(Double rateWeight) |
| `QuoteID` | `String` | Optional | The unique quote identifier for freight based transactions. | String getQuoteID() | setQuoteID(String quoteID) |
| `OptionID` | `String` | Optional | The unique option identifier for freight based transactions. | String getOptionID() | setOptionID(String optionID) |
| `ShipDate` | `String` | Optional | Date the items where shipped. | String getShipDate() | setShipDate(String shipDate) |
| `DeliveryDate` | `String` | Optional | The requested delivery date for the shipment. | String getDeliveryDate() | setDeliveryDate(String deliveryDate) |
| `DeliveryTime` | `String` | Optional | If available the delivery time for the item. | String getDeliveryTime() | setDeliveryTime(String deliveryTime) |
| `DeliveryIn` | `Integer` | Optional | Returned by the carrier indicating the number of days the shipment will take to reach its destination.<br><br>**Default**: `0` | Integer getDeliveryIn() | setDeliveryIn(Integer deliveryIn) |
| `DisplayRate` | `Boolean` | Optional | Indicates if the rate is marked for display to the user.<br><br>**Default**: `false` | Boolean getDisplayRate() | setDisplayRate(Boolean displayRate) |
| `UpdateRate` | `Boolean` | Optional | Indicates if the rate is used during updates back to customer host systems.<br><br>**Default**: `false` | Boolean getUpdateRate() | setUpdateRate(Boolean updateRate) |
| `BuyRate` | `Boolean` | Optional | Indicates if the rate is descignated as the Buy Rate for the external system that submitted the ship request.<br><br>**Default**: `false` | Boolean getBuyRate() | setBuyRate(Boolean buyRate) |
| `SellRate` | `Boolean` | Optional | Indicates if the rate is descignated as the Sell Rate for the external system that submitted the ship request.<br><br>**Default**: `false` | Boolean getSellRate() | setSellRate(Boolean sellRate) |
| `ServiceType` | `Integer` | Optional | Numeric identifier for the carrier service assocaited with the transaction.<br><br>**Default**: `0` | Integer getServiceType() | setServiceType(Integer serviceType) |
| `ChargeGroups` | [`ChargeGroups6`](../../doc/models/charge-groups-6.md) | Optional | Container for all charge groups associated with the transaction. | ChargeGroups6 getChargeGroups() | setChargeGroups(ChargeGroups6 chargeGroups) |

## Example (as XML)

```xml
<wtg:Rate xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:RateWeight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:RateWeight>
  <wtg:DeliveryIn xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:DeliveryIn>
  <wtg:DisplayRate xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DisplayRate>
  <wtg:UpdateRate xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:UpdateRate>
  <wtg:BuyRate xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:BuyRate>
  <wtg:SellRate xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SellRate>
  <wtg:ServiceType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ServiceType>
  <wtg:RateType xmlns:wtg="https://www.wisetechglobal.com/">176</wtg:RateType>
  <wtg:RateDescription xmlns:wtg="https://www.wisetechglobal.com/">RateDescription0</wtg:RateDescription>
  <wtg:QuoteID xmlns:wtg="https://www.wisetechglobal.com/">QuoteID2</wtg:QuoteID>
  <wtg:OptionID xmlns:wtg="https://www.wisetechglobal.com/">OptionID6</wtg:OptionID>
</wtg:Rate>
```

