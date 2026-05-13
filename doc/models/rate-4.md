
# Rate 4

Container for an individual rate.

## Structure

`Rate4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RateType` | `Integer` | Optional | Numeric identifier for the rate type.<br><br>**Default**: `0` | Integer getRateType() | setRateType(Integer rateType) |
| `RateDescription` | `String` | Optional | Free form description for the rate type. | String getRateDescription() | setRateDescription(String rateDescription) |
| `RateWeight` | `Double` | Optional | The rated weight for the package.<br><br>**Default**: `0d` | Double getRateWeight() | setRateWeight(Double rateWeight) |
| `QuoteID` | `String` | Optional | The unique quote identifier for freight based transactions. | String getQuoteID() | setQuoteID(String quoteID) |
| `OptionID` | `String` | Optional | The unique option identifier for freight based transactions. | String getOptionID() | setOptionID(String optionID) |
| `ShipDate` | `String` | Optional | Date the items are to be shipped. Defaults to current date if not submitted. | String getShipDate() | setShipDate(String shipDate) |
| `DeliveryDate` | `String` | Optional | The requested delivery date for the shipment. | String getDeliveryDate() | setDeliveryDate(String deliveryDate) |
| `DisplayRate` | `Boolean` | Optional | Indicates if the rate is marked for display to the user.<br><br>**Default**: `false` | Boolean getDisplayRate() | setDisplayRate(Boolean displayRate) |
| `UpdateRate` | `Boolean` | Optional | Indicates if the rate is used during updates back to customer host systems.<br><br>**Default**: `false` | Boolean getUpdateRate() | setUpdateRate(Boolean updateRate) |
| `ChargeGroups` | [`ChargeGroups2`](../../doc/models/charge-groups-2.md) | Optional | Container for all charge groups associated with the transaction. | ChargeGroups2 getChargeGroups() | setChargeGroups(ChargeGroups2 chargeGroups) |

## Example (as XML)

```xml
<wtg:Rate xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:RateType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:RateType>
  <wtg:RateWeight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:RateWeight>
  <wtg:DisplayRate xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DisplayRate>
  <wtg:UpdateRate xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:UpdateRate>
  <wtg:RateDescription xmlns:wtg="https://www.wisetechglobal.com/">RateDescription4</wtg:RateDescription>
  <wtg:QuoteID xmlns:wtg="https://www.wisetechglobal.com/">QuoteID8</wtg:QuoteID>
  <wtg:OptionID xmlns:wtg="https://www.wisetechglobal.com/">OptionID0</wtg:OptionID>
</wtg:Rate>
```

