
# Rate

Container for an individual rate.

## Structure

`Rate`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RateType` | `int` | Required | Numeric identifier for the rate type. | int getRateType() | setRateType(int rateType) |
| `RateDescription` | `String` | Optional | Free form description for the rate type. | String getRateDescription() | setRateDescription(String rateDescription) |
| `RateWeight` | `Double` | Optional | The rated weight for the package.<br><br>**Default**: `0d` | Double getRateWeight() | setRateWeight(Double rateWeight) |
| `QuoteID` | `String` | Optional | The unique quote identifier for freight based transactions. | String getQuoteID() | setQuoteID(String quoteID) |
| `OptionID` | `String` | Optional | The unique option identifier for freight based transactions. | String getOptionID() | setOptionID(String optionID) |
| `ShipDate` | `String` | Optional | Date the items where shipped. | String getShipDate() | setShipDate(String shipDate) |
| `DeliveryDate` | `String` | Optional | The requested delivery date for the shipment. | String getDeliveryDate() | setDeliveryDate(String deliveryDate) |
| `DeliveryTime` | `String` | Optional | If available the delivery time for the item. | String getDeliveryTime() | setDeliveryTime(String deliveryTime) |
| `DeliveryIn` | `Integer` | Optional | Returned by the carrier indicating the number of days the shipment will take to reach its destination.<br><br>**Default**: `0` | Integer getDeliveryIn() | setDeliveryIn(Integer deliveryIn) |
| `Interline` | `Boolean` | Optional | Indicates whether the shipment requires interline.<br><br>**Default**: `false` | Boolean getInterline() | setInterline(Boolean interline) |
| `Expedited` | `Boolean` | Optional | Indicates whether the shipment requires an expedited service.<br><br>**Default**: `false` | Boolean getExpedited() | setExpedited(Boolean expedited) |
| `DisplayRate` | `Boolean` | Optional | Indicates if the rate is marked for display to the user.<br><br>**Default**: `false` | Boolean getDisplayRate() | setDisplayRate(Boolean displayRate) |
| `UpdateRate` | `Boolean` | Optional | Indicates if the rate is used during updates back to customer host systems.<br><br>**Default**: `false` | Boolean getUpdateRate() | setUpdateRate(Boolean updateRate) |
| `ServiceType` | `Integer` | Optional | Numeric identifier for the carrier service assocaited with the transaction.<br><br>**Default**: `0` | Integer getServiceType() | setServiceType(Integer serviceType) |
| `ChargeGroups` | [`ChargeGroups`](../../doc/models/charge-groups.md) | Required | Container for all charge groups associated with the transaction. | ChargeGroups getChargeGroups() | setChargeGroups(ChargeGroups chargeGroups) |

## Example (as XML)

```xml
<wtg:Rate xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:RateType xmlns:wtg="https://www.wisetechglobal.com/"></wtg:RateType>
  <wtg:RateWeight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:RateWeight>
  <wtg:DeliveryIn xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:DeliveryIn>
  <wtg:Interline xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Interline>
  <wtg:Expedited xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Expedited>
  <wtg:DisplayRate xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DisplayRate>
  <wtg:UpdateRate xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:UpdateRate>
  <wtg:ServiceType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ServiceType>
  <wtg:ChargeGroups xmlns:wtg="https://www.wisetechglobal.com/"></wtg:ChargeGroups>
  <wtg:RateDescription xmlns:wtg="https://www.wisetechglobal.com/">RateDescription2</wtg:RateDescription>
  <wtg:QuoteID xmlns:wtg="https://www.wisetechglobal.com/">QuoteID0</wtg:QuoteID>
  <wtg:OptionID xmlns:wtg="https://www.wisetechglobal.com/">OptionID8</wtg:OptionID>
  <wtg:ShipDate xmlns:wtg="https://www.wisetechglobal.com/">ShipDate2</wtg:ShipDate>
</wtg:Rate>
```

