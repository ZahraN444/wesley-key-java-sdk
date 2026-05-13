
# Commercial Invoice

Container to allow the customization of the commercial invoice details associated with the transaction.

## Structure

`CommercialInvoice`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FreightCharge` | `Double` | Optional | The freight charge to be printed on the commercial invoice.<br><br>**Default**: `0d` | Double getFreightCharge() | setFreightCharge(Double freightCharge) |
| `InsuranceCharge` | `Double` | Optional | The insurance charge to be printed on the commercial invoice.<br><br>**Default**: `0d` | Double getInsuranceCharge() | setInsuranceCharge(Double insuranceCharge) |
| `OtherCharge` | `Double` | Optional | The unclassified charge to be printed on the commercial invoice.<br><br>**Default**: `0d` | Double getOtherCharge() | setOtherCharge(Double otherCharge) |
| `Comments` | `String` | Optional | Comments to be shown on the commercial invoice. | String getComments() | setComments(String comments) |
| `Purpose` | [`PurposeEnum`](../../doc/models/purpose-enum.md) | Optional | The purpose to be shown on the commercial invoice for the consolidated shipment. | PurposeEnum getPurpose() | setPurpose(PurposeEnum purpose) |
| `DeclarationStatement` | `String` | Optional | Declaration Statement to be shown on the commercial invoice. | String getDeclarationStatement() | setDeclarationStatement(String declarationStatement) |
| `OriginatorName` | `String` | Optional | Originator Name to be shown on the commercial invoice. | String getOriginatorName() | setOriginatorName(String originatorName) |
| `SpecialInstructions` | `String` | Optional | Special Instructions to be shown on the commercial invoice. | String getSpecialInstructions() | setSpecialInstructions(String specialInstructions) |

## Example (as XML)

```xml
<wtg:CommercialInvoice xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:FreightCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:FreightCharge>
  <wtg:InsuranceCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:InsuranceCharge>
  <wtg:OtherCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:OtherCharge>
  <wtg:Comments xmlns:wtg="https://www.wisetechglobal.com/">Comments0</wtg:Comments>
  <wtg:Purpose xmlns:wtg="https://www.wisetechglobal.com/">1</wtg:Purpose>
</wtg:CommercialInvoice>
```

