
# Freight 2

Container for freight specific values

## Structure

`Freight2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Billing` | [`Billing5`](../../doc/models/billing-5.md) | Optional | Container for freight billing details associated with the transaction. | Billing5 getBilling() | setBilling(Billing5 billing) |
| `CollectTermsType` | [`CollectTermsTypeEnum`](../../doc/models/collect-terms-type-enum.md) | Optional | Parameter used to set collect terms type | CollectTermsTypeEnum getCollectTermsType() | setCollectTermsType(CollectTermsTypeEnum collectTermsType) |
| `LiabilityCoverageDetail` | `Double` | Optional | Identifies the Liability Coverage Amount per pound | Double getLiabilityCoverageDetail() | setLiabilityCoverageDetail(Double liabilityCoverageDetail) |
| `LiabilityCoverageType` | [`LiabilityCoverageTypeEnum`](../../doc/models/liability-coverage-type-enum.md) | Optional | Parameter used to set liability coverage type | LiabilityCoverageTypeEnum getLiabilityCoverageType() | setLiabilityCoverageType(LiabilityCoverageTypeEnum liabilityCoverageType) |
| `PurposeOfShipment` | [`PurposeOfShipmentEnum`](../../doc/models/purpose-of-shipment-enum.md) | Optional | Parameter used to set nature of shipment | PurposeOfShipmentEnum getPurposeOfShipment() | setPurposeOfShipment(PurposeOfShipmentEnum purposeOfShipment) |
| `ClientDiscountPercent` | `Double` | Optional | Estimated discount rate provided by client for unsecured rate quote. | Double getClientDiscountPercent() | setClientDiscountPercent(Double clientDiscountPercent) |
| `FreightCharge` | `Double` | Optional | Identifies the customer charge to assign to the freight shipment | Double getFreightCharge() | setFreightCharge(Double freightCharge) |
| `MiscellaneousCharges` | `Double` | Optional | Identifies an additional tax or miscellaneous charge the customer can assign to the freight shipment | Double getMiscellaneousCharges() | setMiscellaneousCharges(Double miscellaneousCharges) |
| `Comments` | `String` | Optional | Customer assigned comments for a freight shipment. | String getComments() | setComments(String comments) |

## Example (as XML)

```xml
<wtg:Freight xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Billing xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Billing>
  <wtg:CollectTermsType xmlns:wtg="https://www.wisetechglobal.com/">1</wtg:CollectTermsType>
  <wtg:LiabilityCoverageDetail xmlns:wtg="https://www.wisetechglobal.com/">55</wtg:LiabilityCoverageDetail>
  <wtg:LiabilityCoverageType xmlns:wtg="https://www.wisetechglobal.com/">1</wtg:LiabilityCoverageType>
  <wtg:PurposeOfShipment xmlns:wtg="https://www.wisetechglobal.com/">5</wtg:PurposeOfShipment>
</wtg:Freight>
```

