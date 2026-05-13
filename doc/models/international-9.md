
# International 9

Container for international details associated with the shipment.

## Structure

`International9`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ReceiverCustomsIdentificationNumber` | `String` | Optional | Customs Identification number of the receiver. | String getReceiverCustomsIdentificationNumber() | setReceiverCustomsIdentificationNumber(String receiverCustomsIdentificationNumber) |
| `ReceiverCustomsIdentificationType` | [`ReceiverCustomsIdentificationTypeEnum`](../../doc/models/receiver-customs-identification-type-enum.md) | Optional | Customs Identification Type of the receiver.. | ReceiverCustomsIdentificationTypeEnum getReceiverCustomsIdentificationType() | setReceiverCustomsIdentificationType(ReceiverCustomsIdentificationTypeEnum receiverCustomsIdentificationType) |
| `CustomsInsuranceChargesValue` | `Double` | Optional | Customs Insurance Charges value. | Double getCustomsInsuranceChargesValue() | setCustomsInsuranceChargesValue(Double customsInsuranceChargesValue) |
| `CustomsInsuranceChargesCurrency` | `String` | Optional | Customs Insurance Charges currency. | String getCustomsInsuranceChargesCurrency() | setCustomsInsuranceChargesCurrency(String customsInsuranceChargesCurrency) |
| `IsInternational` | `Boolean` | Optional | Indicates whether the package is part of an international shipment.  Defaults to no if omitted.<br><br>**Default**: `false` | Boolean getIsInternational() | setIsInternational(Boolean isInternational) |
| `NonDutiable` | `Boolean` | Optional | Indicates whether the package contains only non-dutiable goods.  Defaults to no if omitted.<br><br>**Default**: `false` | Boolean getNonDutiable() | setNonDutiable(Boolean nonDutiable) |
| `DocumentsOnly` | `Boolean` | Optional | Indicates whether the package contains only documents.  Defaults to not documents only if omitted.<br><br>**Default**: `false` | Boolean getDocumentsOnly() | setDocumentsOnly(Boolean documentsOnly) |
| `PrePackedBoxes` | [`PrePackedBoxes`](../../doc/models/pre-packed-boxes.md) | Optional | pre-packed boxes, including any items specified that will be packed and excess space used before any new boxes are created. | PrePackedBoxes getPrePackedBoxes() | setPrePackedBoxes(PrePackedBoxes prePackedBoxes) |
| `Contents` | [`Contents6`](../../doc/models/contents-6.md) | Optional | Container for all contents (line items) associated with the transaction. | Contents6 getContents() | setContents(Contents6 contents) |

## Example (as XML)

```xml
<wtg:International xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:IsInternational xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:IsInternational>
  <wtg:NonDutiable xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NonDutiable>
  <wtg:DocumentsOnly xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DocumentsOnly>
  <wtg:ReceiverCustomsIdentificationNumber xmlns:wtg="https://www.wisetechglobal.com/">ReceiverCustomsIdentificationNumber4</wtg:ReceiverCustomsIdentificationNumber>
  <wtg:ReceiverCustomsIdentificationType xmlns:wtg="https://www.wisetechglobal.com/">1</wtg:ReceiverCustomsIdentificationType>
  <wtg:CustomsInsuranceChargesValue xmlns:wtg="https://www.wisetechglobal.com/">194.64</wtg:CustomsInsuranceChargesValue>
  <wtg:CustomsInsuranceChargesCurrency xmlns:wtg="https://www.wisetechglobal.com/">CustomsInsuranceChargesCurrency8</wtg:CustomsInsuranceChargesCurrency>
</wtg:International>
```

