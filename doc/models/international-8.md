
# International 8

Container for international details associated with the shipment.

## Structure

`International8`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Duty` | [`Duty2`](../../doc/models/duty-2.md) | Optional | Container for duty details assocaited with the transaction. | Duty2 getDuty() | setDuty(Duty2 duty) |
| `Broker` | [`Broker1`](../../doc/models/broker-1.md) | Optional | Container for broker details. | Broker1 getBroker() | setBroker(Broker1 broker) |
| `AssociateWithReturn` | `Boolean` | Optional | Indicator that this shipment is to be associated with a return shipment. Defaults to no.<br><br>**Default**: `false` | Boolean getAssociateWithReturn() | setAssociateWithReturn(Boolean associateWithReturn) |
| `CustomsReturnReasonID` | `Integer` | Optional | In cases where an International outbound shipment is to associated with a return shipment. This is the customs reason for the outbound shipment.<br><br>**Default**: `0` | Integer getCustomsReturnReasonID() | setCustomsReturnReasonID(Integer customsReturnReasonID) |
| `CustomsReturnReasonDescription` | `String` | Optional | In cases where a standard return reason is not suitable then this field can be populated with a free form reason. Will be ignored unless Customs Return Reason Identifier is set to Other. This is the reason for the outbound shipment. | String getCustomsReturnReasonDescription() | setCustomsReturnReasonDescription(String customsReturnReasonDescription) |
| `ReceiverIdentificationNumber` | `String` | Optional | Tax Identification number of the receiver. | String getReceiverIdentificationNumber() | setReceiverIdentificationNumber(String receiverIdentificationNumber) |
| `ReceiverIdentificationType` | `String` | Optional | Tax Identification Type of the receiver. | String getReceiverIdentificationType() | setReceiverIdentificationType(String receiverIdentificationType) |
| `UltimateDestinationCountry` | `String` | Optional | Ultimate destination country of the shipment. | String getUltimateDestinationCountry() | setUltimateDestinationCountry(String ultimateDestinationCountry) |
| `SenderReceiverRelated` | `Boolean` | Optional | Indicates whether the sender and receiver of the shipment and related.  Defaults to not related if not submitted.<br><br>**Default**: `false` | Boolean getSenderReceiverRelated() | setSenderReceiverRelated(Boolean senderReceiverRelated) |
| `TotalDutyValue` | `Double` | Optional | Declared total export value.<br><br>**Default**: `0d` | Double getTotalDutyValue() | setTotalDutyValue(Double totalDutyValue) |
| `TotalDutyValueCurrency` | `String` | Optional | Currency for the declared total export value. | String getTotalDutyValueCurrency() | setTotalDutyValueCurrency(String totalDutyValueCurrency) |
| `ExportTransactionNumber` | `String` | Optional | Export Transaction Number Issued by the official export body e.g. AES/ ATLAS. | String getExportTransactionNumber() | setExportTransactionNumber(String exportTransactionNumber) |
| `AESTransactionNumber` | `String` | Optional | Transaction number of the shipment's online Shipper's Export Declaration (SED) filing. | String getAESTransactionNumber() | setAESTransactionNumber(String aESTransactionNumber) |
| `AESEntryNumber` | `String` | Optional | AES entry number to use with this shipment. | String getAESEntryNumber() | setAESEntryNumber(String aESEntryNumber) |
| `B13ATransactionNumber` | `String` | Optional | Transaction number of the shipment's B13A filing. | String getB13ATransactionNumber() | setB13ATransactionNumber(String b13ATransactionNumber) |
| `TermsOfSale` | `Integer` | Optional | Rights and obligations of each party when it comes to transporting the shipment.<br><br>**Default**: `0` | Integer getTermsOfSale() | setTermsOfSale(Integer termsOfSale) |
| `TermsOfSaleConsigneeAccountNumber` | `String` | Optional | The account number to which the consignee's costs (that are determined by the selected Terms Of Sale) are charged. | String getTermsOfSaleConsigneeAccountNumber() | setTermsOfSaleConsigneeAccountNumber(String termsOfSaleConsigneeAccountNumber) |
| `FreeFormTermsOfSale` | `String` | Optional | The Terms Of Sale entered by the user. | String getFreeFormTermsOfSale() | setFreeFormTermsOfSale(String freeFormTermsOfSale) |
| `BookingNumber` | `Integer` | Optional | Booking number for the shipment.<br><br>**Default**: `0` | Integer getBookingNumber() | setBookingNumber(Integer bookingNumber) |
| `UltimateConsignee` | [`UltimateConsignee2`](../../doc/models/ultimate-consignee-2.md) | Optional | Container to allow the customization of the ultimate consignee address details associated with the transaction. | UltimateConsignee2 getUltimateConsignee() | setUltimateConsignee(UltimateConsignee2 ultimateConsignee) |
| `Origin` | [`Origin`](../../doc/models/origin.md) | Optional | Container for origin details. | Origin getOrigin() | setOrigin(Origin origin) |
| `FreightForwarder` | [`FreightForwarder1`](../../doc/models/freight-forwarder-1.md) | Optional | Container to allow the customization of the freight forwarder address details associated with the transaction. | FreightForwarder1 getFreightForwarder() | setFreightForwarder(FreightForwarder1 freightForwarder) |
| `ExportReason` | `Integer` | Optional | Reason for exporting the shipment. Defaults to None or the configured value in International Defaults.<br><br>**Default**: `0` | Integer getExportReason() | setExportReason(Integer exportReason) |
| `ExportCode` | `String` | Optional | Code associated with the export reason. | String getExportCode() | setExportCode(String exportCode) |
| `ExportDeclaration` | `String` | Optional | Declaration associated with the export reason. | String getExportDeclaration() | setExportDeclaration(String exportDeclaration) |
| `IdentificationType` | `Integer` | Optional | Export organization identifier type.<br><br>**Default**: `0` | Integer getIdentificationType() | setIdentificationType(Integer identificationType) |
| `Identifier` | `String` | Optional | Export organization identifier. | String getIdentifier() | setIdentifier(String identifier) |
| `ExportLicense` | `String` | Optional | Export license number. | String getExportLicense() | setExportLicense(String exportLicense) |
| `ExportLicenseExpires` | `String` | Optional | Date the export expires. | String getExportLicenseExpires() | setExportLicenseExpires(String exportLicenseExpires) |
| `ImportLicense` | `String` | Optional | Import license number. | String getImportLicense() | setImportLicense(String importLicense) |
| `ImportLicenseExpires` | `String` | Optional | Date the import license expires. | String getImportLicenseExpires() | setImportLicenseExpires(String importLicenseExpires) |
| `CanadaExportPermitNumber` | `String` | Optional | Canadian export permit number. | String getCanadaExportPermitNumber() | setCanadaExportPermitNumber(String canadaExportPermitNumber) |
| `InternationalControlledExportLicenseType` | [`InternationalControlledExportLicenseTypeEnum`](../../doc/models/international-controlled-export-license-type-enum.md) | Optional | International controlled export license type. | InternationalControlledExportLicenseTypeEnum getInternationalControlledExportLicenseType() | setInternationalControlledExportLicenseType(InternationalControlledExportLicenseTypeEnum internationalControlledExportLicenseType) |
| `InternationalControlledExportLicenseNumber` | `String` | Optional | International controlled export license number. | String getInternationalControlledExportLicenseNumber() | setInternationalControlledExportLicenseNumber(String internationalControlledExportLicenseNumber) |
| `InternationalControlledExportLicenseExpiryDate` | `String` | Optional | International controlled export license expiry date. | String getInternationalControlledExportLicenseExpiryDate() | setInternationalControlledExportLicenseExpiryDate(String internationalControlledExportLicenseExpiryDate) |
| `InternationalControlledExportTradeZone` | `String` | Optional | International controlled export trade foreign trade zone. | String getInternationalControlledExportTradeZone() | setInternationalControlledExportTradeZone(String internationalControlledExportTradeZone) |
| `InternationalControlledExportEntryNumber` | `String` | Optional | International controlled export entry number. | String getInternationalControlledExportEntryNumber() | setInternationalControlledExportEntryNumber(String internationalControlledExportEntryNumber) |
| `B13A` | [`B13A`](../../doc/models/b13-a.md) | Optional | Container for B13A details. | B13A getB13A() | setB13A(B13A b13A) |
| `SED` | [`SED`](../../doc/models/sed.md) | Optional | Container for SED details. | SED getSED() | setSED(SED sED) |
| `ExcludeFromConsolidation` | `Boolean` | Optional | Parameter used to set the shipment as excluded from any consolidation. Defaults to the false. | Boolean getExcludeFromConsolidation() | setExcludeFromConsolidation(Boolean excludeFromConsolidation) |
| `SenderSignatureName` | `String` | Optional | Sender signature name to appear on qualifying international shipping document(s). | String getSenderSignatureName() | setSenderSignatureName(String senderSignatureName) |

## Example (as XML)

```xml
<wtg:International xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:AssociateWithReturn xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AssociateWithReturn>
  <wtg:CustomsReturnReasonID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:CustomsReturnReasonID>
  <wtg:SenderReceiverRelated xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SenderReceiverRelated>
  <wtg:TotalDutyValue xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TotalDutyValue>
  <wtg:TermsOfSale xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TermsOfSale>
  <wtg:BookingNumber xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:BookingNumber>
  <wtg:ExportReason xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ExportReason>
  <wtg:IdentificationType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:IdentificationType>
  <wtg:Duty xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Duty>
  <wtg:Broker xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Broker>
  <wtg:CustomsReturnReasonDescription xmlns:wtg="https://www.wisetechglobal.com/">CustomsReturnReasonDescription4</wtg:CustomsReturnReasonDescription>
</wtg:International>
```

