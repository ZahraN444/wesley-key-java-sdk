
# Pierbridge Ship Request

Processes a shipment with a carrier.

## Structure

`PierbridgeShipRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `UpdateShipmentType` | [`UpdateShipmentTypeEnum`](../../doc/models/update-shipment-type-enum.md) | Optional | Indicator of the type of update being performed on the shipment.<br><br>**Default**: `UpdateShipmentTypeEnum.NONE` | UpdateShipmentTypeEnum getUpdateShipmentType() | setUpdateShipmentType(UpdateShipmentTypeEnum updateShipmentType) |
| `UpdateShipmentID` | `Integer` | Optional | Identifier of the Shipment to be updated. To be used in conjunction with the UpdateShipmentType element.<br><br>**Default**: `0` | Integer getUpdateShipmentID() | setUpdateShipmentID(Integer updateShipmentID) |
| `DisplayRateTypeID` | `Integer` | Optional | Identifier of the rate used for display to the user.<br><br>**Default**: `0` | Integer getDisplayRateTypeID() | setDisplayRateTypeID(Integer displayRateTypeID) |
| `UpdateRateTypeID` | `Integer` | Optional | Identifier of the rate used to update the host system.<br><br>**Default**: `0` | Integer getUpdateRateTypeID() | setUpdateRateTypeID(Integer updateRateTypeID) |
| `OtherRateTypeID` | `Integer` | Optional | Identifier of any other rate required in the response.<br><br>**Default**: `0` | Integer getOtherRateTypeID() | setOtherRateTypeID(Integer otherRateTypeID) |
| `OtherRateTypes` | [`OtherRateTypes`](../../doc/models/other-rate-types.md) | Optional | Container for the additional rate types to be requested by the transaction. | OtherRateTypes getOtherRateTypes() | setOtherRateTypes(OtherRateTypes otherRateTypes) |
| `IsReturn` | `Boolean` | Optional | Identifier to indicate that this is a rate for a return shipment. This flag is only supported by a limited number of carriers.<br><br>**Default**: `false` | Boolean getIsReturn() | setIsReturn(Boolean isReturn) |
| `DisableValidation` | `Boolean` | Optional | Indicates whether to disable the internal validation rules for this request.<br><br>**Default**: `false` | Boolean getDisableValidation() | setDisableValidation(Boolean disableValidation) |
| `DisableExecution` | `Boolean` | Optional | Indicates whether to disable the actual execution with the carrier engine for this request. Use with caution, the shipment will be recorded in the system but not executed with the carrier. Rating can be passed manually or executed with Rating Options.<br><br>**Default**: `false` | Boolean getDisableExecution() | setDisableExecution(Boolean disableExecution) |
| `ExportInvoiceData` | `Boolean` | Optional | Indicates whether to include the shipment charges in invoice data export to CW1<br><br>**Default**: `false` | Boolean getExportInvoiceData() | setExportInvoiceData(Boolean exportInvoiceData) |
| `InvoiceDebtor` | [`InvoiceDebtor`](../../doc/models/invoice-debtor.md) | Optional | Container for invoice debtor details associated with the transaction. | InvoiceDebtor getInvoiceDebtor() | setInvoiceDebtor(InvoiceDebtor invoiceDebtor) |
| `ResetWayBillNumbers` | `Boolean` | Optional | Indicates whether to reset any manually passed in values within the WayBillNumber element for both the current request and any associated cached packages already added with the package request.<br><br>**Default**: `false` | Boolean getResetWayBillNumbers() | setResetWayBillNumbers(Boolean resetWayBillNumbers) |
| `ReverseSenderReceiverAddress` | `Boolean` | Optional | Indicates whether to reverse the addresses past in the Sender and Receiver blocks to effectively process this as a shipment but in reverse. Not to be confused with the return request.<br><br>**Default**: `false` | Boolean getReverseSenderReceiverAddress() | setReverseSenderReceiverAddress(Boolean reverseSenderReceiverAddress) |
| `UserName` | `String` | Required | The user name to use when processing the transaction. | String getUserName() | setUserName(String userName) |
| `Batch` | `Integer` | Optional | Internal node, set by shipments server during Batch processing. Do not use or set. | Integer getBatch() | setBatch(Integer batch) |
| `ServiceTypeAlternateCount` | `Integer` | Optional | Internal node. Do not use or set. | Integer getServiceTypeAlternateCount() | setServiceTypeAlternateCount(Integer serviceTypeAlternateCount) |
| `ShipmentGroupID` | `Integer` | Optional | Internal node, set by shipments server during Batch processing. Do not use or set. | Integer getShipmentGroupID() | setShipmentGroupID(Integer shipmentGroupID) |
| `CustomRateEngineKey1` | `String` | Optional | Custom pass through value for Custom Rate Engines. | String getCustomRateEngineKey1() | setCustomRateEngineKey1(String customRateEngineKey1) |
| `CustomRateEngineKey2` | `String` | Optional | Custom pass through value for Custom Rate Engines. | String getCustomRateEngineKey2() | setCustomRateEngineKey2(String customRateEngineKey2) |
| `CustomRateEngineKey3` | `String` | Optional | Custom pass through value for Custom Rate Engines. | String getCustomRateEngineKey3() | setCustomRateEngineKey3(String customRateEngineKey3) |
| `BrokerReference` | `String` | Optional | Broker reference. | String getBrokerReference() | setBrokerReference(String brokerReference) |
| `ISOCurrencyId` | `Integer` | Optional | The ID of the ISO Currency code in use.<br><br>**Default**: `0` | Integer getISOCurrencyId() | setISOCurrencyId(Integer iSOCurrencyId) |
| `Trailer` | `String` | Optional | Free entry field used to refer to which trailer shipments have been committed to. | String getTrailer() | setTrailer(String trailer) |
| `DocketConsolidation` | `Boolean` | Optional | Indicates that the shipment should be under the docket code. This docket code is set in the Billing Account number field when this flag is used.<br><br>**Default**: `false` | Boolean getDocketConsolidation() | setDocketConsolidation(Boolean docketConsolidation) |
| `RecordIdentifiers` | [`RecordIdentifiers`](../../doc/models/record-identifiers.md) | Optional | Outer container for transaction identifiers. | RecordIdentifiers getRecordIdentifiers() | setRecordIdentifiers(RecordIdentifiers recordIdentifiers) |
| `BOLHandling` | [`BOLHandling`](../../doc/models/bol-handling.md) | Optional | Container to allow handling of BOL to be specified. | BOLHandling getBOLHandling() | setBOLHandling(BOLHandling bOLHandling) |
| `OutputHandling` | [`OutputHandling`](../../doc/models/output-handling.md) | Optional | Container to allow handling of outputs to be specified. | OutputHandling getOutputHandling() | setOutputHandling(OutputHandling outputHandling) |
| `Outputs` | [`Outputs`](../../doc/models/outputs.md) | Optional | Container for outputs the transaction should generate or customize the printing of. | Outputs getOutputs() | setOutputs(Outputs outputs) |
| `Quote` | [`Quote`](../../doc/models/quote.md) | Optional | Container for quote information. | Quote getQuote() | setQuote(Quote quote) |
| `Orders` | [`Orders1`](../../doc/models/orders-1.md) | Optional | Container all orders associated with the transaction. | Orders1 getOrders() | setOrders(Orders1 orders) |
| `IsWorldEase` | `Boolean` | Optional | Indicates if the shipment should use UPS WorldEase.<br><br>**Default**: `false` | Boolean getIsWorldEase() | setIsWorldEase(Boolean isWorldEase) |
| `WorldEaseCode` | `String` | Optional | UPS WorldEase Code. | String getWorldEaseCode() | setWorldEaseCode(String worldEaseCode) |
| `ThirdPartyHazardous` | [`ThirdPartyHazardous3`](../../doc/models/third-party-hazardous-3.md) | Optional | Container for details for processing by an external hazardous compliance system. | ThirdPartyHazardous3 getThirdPartyHazardous() | setThirdPartyHazardous(ThirdPartyHazardous3 thirdPartyHazardous) |
| `ImporterOfRecord` | [`ImporterOfRecord`](../../doc/models/importer-of-record.md) | Optional | Container for importer of record details. | ImporterOfRecord getImporterOfRecord() | setImporterOfRecord(ImporterOfRecord importerOfRecord) |
| `CommercialInvoicePaperless` | `Boolean` | Optional | Indicates whether the Commercial Invoice for this shipment is going to be submitted electronically.  Defaults to not paperless if not submitted.<br><br>**Default**: `false` | Boolean getCommercialInvoicePaperless() | setCommercialInvoicePaperless(Boolean commercialInvoicePaperless) |
| `CertificateOfOriginPaperless` | `Boolean` | Optional | Indicates whether the Certificate Of Origin for this shipment is going to be submitted electronically.  Defaults to not paperless if not submitted.<br><br>**Default**: `false` | Boolean getCertificateOfOriginPaperless() | setCertificateOfOriginPaperless(Boolean certificateOfOriginPaperless) |
| `PaperlessDocumentReference` | `String` | Optional | Document reference sent to carrier when using electronic trade documents. | String getPaperlessDocumentReference() | setPaperlessDocumentReference(String paperlessDocumentReference) |
| `CommercialInvoiceWithheld` | `Boolean` | Optional | Indicates whether the Commercial Invoice for this shipment should not be attached to the delivery.  Defaults to false.<br><br>**Default**: `false` | Boolean getCommercialInvoiceWithheld() | setCommercialInvoiceWithheld(Boolean commercialInvoiceWithheld) |
| `AdditionalHardcopyDocumentation` | `Boolean` | Optional | Indicates whether any hardcopy documents accompany the shipment in addition to any paperless document.  Defaults to no additional hardcopy documents if not submitted.<br><br>**Default**: `false` | Boolean getAdditionalHardcopyDocumentation() | setAdditionalHardcopyDocumentation(Boolean additionalHardcopyDocumentation) |
| `RateGroup` | `Integer` | Optional | Rate group to use for the rate shop.<br><br>**Default**: `0` | Integer getRateGroup() | setRateGroup(Integer rateGroup) |
| `RateGroupName` | `String` | Optional | Rate Group Name to use for the rate shop. | String getRateGroupName() | setRateGroupName(String rateGroupName) |
| `FilterMode` | `Integer` | Optional | Determines what filtering is applied to the returned rates.  1 = select cheapest rate only for RateGroup; 2 = select cheapest rate that meets required date and time for RateGroup; 3 = use SortMode to determine which rate selected from SCACs in the Filter SCAC elements; 4 = use SortMode to determine which rate selected from SCACs in the Filter Service SCAC elements.<br><br>**Default**: `0` | Integer getFilterMode() | setFilterMode(Integer filterMode) |
| `SortMode` | `Integer` | Optional | Determines which rate is selected from the returned rates when using FilterSCACs or FilterServiceSCACs.  1 = select cheapest rate only; 2 = select cheapest rate that meets required date and time; Only used when FilterMode = 3 or 4.<br><br>**Default**: `0` | Integer getSortMode() | setSortMode(Integer sortMode) |
| `FilterSCACs` | [`FilterSCACs`](../../doc/models/filter-sca-cs.md) | Optional | Container element carrier SCAC codes used to filter the results. | FilterSCACs getFilterSCACs() | setFilterSCACs(FilterSCACs filterSCACs) |
| `FilterServiceSCACs` | [`FilterServiceSCACs`](../../doc/models/filter-service-sca-cs.md) | Optional | Container element carrier service SCAC codes used to filter the results. | FilterServiceSCACs getFilterServiceSCACs() | setFilterServiceSCACs(FilterServiceSCACs filterServiceSCACs) |
| `InsuranceProvider` | `Integer` | Optional | Company that is to provide the insurance for the shipment.  Only provide a value if you are using a third party insurer.<br><br>**Default**: `0` | Integer getInsuranceProvider() | setInsuranceProvider(Integer insuranceProvider) |
| `CustomCarrierCode` | `String` | Optional | Custom code that relates to the selected options (e.g. carrier, service, package). | String getCustomCarrierCode() | setCustomCarrierCode(String customCarrierCode) |
| `ShippingNotes` | `String` | Optional | Notes that are to accompany the shipment. | String getShippingNotes() | setShippingNotes(String shippingNotes) |
| `CommercialInvoiceFreeText` | `String` | Optional | Notes for the commercial invoice. | String getCommercialInvoiceFreeText() | setCommercialInvoiceFreeText(String commercialInvoiceFreeText) |
| `PickupInstructions` | `String` | Optional | Instructions relating to the collection/pickup of the shipment. | String getPickupInstructions() | setPickupInstructions(String pickupInstructions) |
| `PurchaseOrderNumber` | `String` | Optional | Purchase order number associated with the transaction. | String getPurchaseOrderNumber() | setPurchaseOrderNumber(String purchaseOrderNumber) |
| `SalesOrderNumber` | `String` | Optional | Sales order number associated with the transaction. | String getSalesOrderNumber() | setSalesOrderNumber(String salesOrderNumber) |
| `PickListNumber` | `String` | Optional | Pick list number associated with the shipment. | String getPickListNumber() | setPickListNumber(String pickListNumber) |
| `ControlIdentifier` | `String` | Optional | A reference to a control which generated the request, this value is not used during processing and will be returned in the response. | String getControlIdentifier() | setControlIdentifier(String controlIdentifier) |
| `TransactionIdentifier` | `String` | Optional | A unique identifier for the transaction, this value is not used during processing and will be returned in the response. | String getTransactionIdentifier() | setTransactionIdentifier(String transactionIdentifier) |
| `Live` | `Boolean` | Optional | Indicates whether the transaction is a test or live.  Defaults to system configured value if not submitted.<br><br>**Default**: `false` | Boolean getLive() | setLive(Boolean live) |
| `MeterSerialNumber` | `String` | Optional | Unique serial number for the meter to add. | String getMeterSerialNumber() | setMeterSerialNumber(String meterSerialNumber) |
| `NumberOfPieces` | `Integer` | Optional | Number of items processed for this transaction.<br><br>**Default**: `0` | Integer getNumberOfPieces() | setNumberOfPieces(Integer numberOfPieces) |
| `PharmacyDelivery` | `Boolean` | Optional | Value indicates shipment is a FedEx pharmacy delivery.<br><br>**Default**: `false` | Boolean getPharmacyDelivery() | setPharmacyDelivery(Boolean pharmacyDelivery) |
| `IORCode` | `String` | Optional | Identifies the Importer of Record facility code for the consolidated shipment. | String getIORCode() | setIORCode(String iORCode) |
| `ConsolidationDataType` | [`ConsolidationDataTypeEnum`](../../doc/models/consolidation-data-type-enum.md) | Optional | Identifies the field being specified for consolidated aggregation | ConsolidationDataTypeEnum getConsolidationDataType() | setConsolidationDataType(ConsolidationDataTypeEnum consolidationDataType) |
| `ConsolidationDataSourceType` | [`ConsolidationDataSourceTypeEnum`](../../doc/models/consolidation-data-source-type-enum.md) | Optional | Identifies how the content of the field should be determined for consolidated aggregation | ConsolidationDataSourceTypeEnum getConsolidationDataSourceType() | setConsolidationDataSourceType(ConsolidationDataSourceTypeEnum consolidationDataSourceType) |
| `DistributionLocationID` | `String` | Optional | Specifies the location id of the distribution location used to process a consolidation | String getDistributionLocationID() | setDistributionLocationID(String distributionLocationID) |
| `DistributionLocationNumber` | `Integer` | Optional | Specifies the location number of the distribution location used to process a consolidation | Integer getDistributionLocationNumber() | setDistributionLocationNumber(Integer distributionLocationNumber) |
| `DistributionLocationType` | [`DistributionLocationTypeEnum`](../../doc/models/distribution-location-type-enum.md) | Optional | Specifies the type  of the distribution location used to process a consolidation | DistributionLocationTypeEnum getDistributionLocationType() | setDistributionLocationType(DistributionLocationTypeEnum distributionLocationType) |
| `InclusionSpecificationsCarrierCode` | [`InclusionSpecificationsCarrierCodeEnum`](../../doc/models/inclusion-specifications-carrier-code-enum.md) | Optional | Specifies the type  of the inclusion specifications carrier code used to process a consolidation | InclusionSpecificationsCarrierCodeEnum getInclusionSpecificationsCarrierCode() | setInclusionSpecificationsCarrierCode(InclusionSpecificationsCarrierCodeEnum inclusionSpecificationsCarrierCode) |
| `InclusionSpecificationsServiceCategory` | [`InclusionSpecificationsServiceCategoryEnum`](../../doc/models/inclusion-specifications-service-category-enum.md) | Optional | Specifies the type  of the inclusion specifications service category used to process a consolidation | InclusionSpecificationsServiceCategoryEnum getInclusionSpecificationsServiceCategory() | setInclusionSpecificationsServiceCategory(InclusionSpecificationsServiceCategoryEnum inclusionSpecificationsServiceCategory) |
| `ConsolidatedDistributionLtlDetail` | [`ConsolidatedDistributionLtlDetail`](../../doc/models/consolidated-distribution-ltl-detail.md) | Optional | Container for details for origin-country LTL services performed by carrier | ConsolidatedDistributionLtlDetail getConsolidatedDistributionLtlDetail() | setConsolidatedDistributionLtlDetail(ConsolidatedDistributionLtlDetail consolidatedDistributionLtlDetail) |
| `CostCenterMode` | [`CostCenterModeEnum`](../../doc/models/cost-center-mode-enum.md) | Optional | Indicates how cost centers are handled whilst processing the transaction. | CostCenterModeEnum getCostCenterMode() | setCostCenterMode(CostCenterModeEnum costCenterMode) |
| `CostCenterID` | `Integer` | Optional | Identifier of the cost center, should pass either this element or the Cost Center Code.<br><br>**Default**: `0` | Integer getCostCenterID() | setCostCenterID(Integer costCenterID) |
| `CostCenterCode` | `String` | Optional | Code of the cost center, should pass either this element or the Cost Center ID. | String getCostCenterCode() | setCostCenterCode(String costCenterCode) |
| `CostCenterBarcodeIndicator` | `Boolean` | Optional | Determines if the CostCenter field will be barcoded at the bottom of the label.<br><br>**Default**: `false` | Boolean getCostCenterBarcodeIndicator() | setCostCenterBarcodeIndicator(Boolean costCenterBarcodeIndicator) |
| `PackageIDBarcodeIndicator` | `Boolean` | Optional | Determines if the PackageID field will be barcoded at the bottom of the label.<br><br>**Default**: `false` | Boolean getPackageIDBarcodeIndicator() | setPackageIDBarcodeIndicator(Boolean packageIDBarcodeIndicator) |
| `AccountCode` | `String` | Optional | Account code for billing. | String getAccountCode() | setAccountCode(String accountCode) |
| `CompanyCode` | `String` | Optional | Company code for billing. | String getCompanyCode() | setCompanyCode(String companyCode) |
| `ShipForUserID` | `Integer` | Optional | User identifier for Ship For user.<br><br>**Default**: `0` | Integer getShipForUserID() | setShipForUserID(Integer shipForUserID) |
| `Carrier` | `int` | Required | Numeric identifier for the carrier.<br><br>**Default**: `0` | int getCarrier() | setCarrier(int carrier) |
| `ServiceType` | `int` | Required | Carrier service (e.g. Next Day, Ground, Express) to ship with.<br><br>**Default**: `0` | int getServiceType() | setServiceType(int serviceType) |
| `PackageType` | `Integer` | Optional | Carrier package (e.g. letter, package, pallet) that is to be shipped.<br><br>**Default**: `0` | Integer getPackageType() | setPackageType(Integer packageType) |
| `SuggestedServiceType` | `Integer` | Optional | Carrier service (e.g. Next Day, Ground, Express) that was recommended by e.g. rate shopping.<br><br>**Default**: `0` | Integer getSuggestedServiceType() | setSuggestedServiceType(Integer suggestedServiceType) |
| `CustomerServiceType` | `Integer` | Optional | Carrier service (e.g. Next Day, Ground, Express) that the customer has paid for.<br><br>**Default**: `0` | Integer getCustomerServiceType() | setCustomerServiceType(Integer customerServiceType) |
| `CustomerCostOption` | `Integer` | Optional | Cost option that is to be applied to the shipping charges.  Used to charge the customer a fixed cost or some multiple of actual shipping charges.<br><br>**Default**: `0` | Integer getCustomerCostOption() | setCustomerCostOption(Integer customerCostOption) |
| `DeliveryWindowId` | `String` | Optional | Carrier unique identifier for a delivery window. | String getDeliveryWindowId() | setDeliveryWindowId(String deliveryWindowId) |
| `ShipDate` | `String` | Optional | Date the items are to be shipped. Defaults to current date if not submitted. | String getShipDate() | setShipDate(String shipDate) |
| `ShipBeforeTime` | `String` | Optional | Time before which the carrier may pickup the shipment. | String getShipBeforeTime() | setShipBeforeTime(String shipBeforeTime) |
| `ShipAfterTime` | `String` | Optional | Time after which the carrier may pickup the shipment. | String getShipAfterTime() | setShipAfterTime(String shipAfterTime) |
| `RequiredDate` | `String` | Optional | Date that the shipment is required to arrive at the receiver. | String getRequiredDate() | setRequiredDate(String requiredDate) |
| `OrderDate` | `String` | Optional | Date associated with the order. | String getOrderDate() | setOrderDate(String orderDate) |
| `SaturdayDelivery` | `Boolean` | Optional | Indicates whether the shipment is intended for delivery on a Saturday.  Defaults to non-Saturday delivery if not submitted.<br><br>**Default**: `false` | Boolean getSaturdayDelivery() | setSaturdayDelivery(Boolean saturdayDelivery) |
| `SaturdayPickup` | `Boolean` | Optional | Indicates whether the shipment is intended for pickup on a Saturday.  Defaults to non-Saturday pickup if not submitted.<br><br>**Default**: `false` | Boolean getSaturdayPickup() | setSaturdayPickup(Boolean saturdayPickup) |
| `SundayPickup` | `Boolean` | Optional | Indicates whether the shipment is intended for pickup on a Sunday.  Defaults to non-Sunday pickup if not submitted.<br><br>**Default**: `false` | Boolean getSundayPickup() | setSundayPickup(Boolean sundayPickup) |
| `AfterHoursDelivery` | `Boolean` | Optional | Indicates whether the shipment will be performed after normal working hours.  Defaults to false if not submitted.<br><br>**Default**: `false` | Boolean getAfterHoursDelivery() | setAfterHoursDelivery(Boolean afterHoursDelivery) |
| `CorrectedBOLFee` | `Boolean` | Optional | Indicates whether a corrected Bill Of Lading fee is applicable.  Defaults to false if not submitted.<br><br>**Default**: `false` | Boolean getCorrectedBOLFee() | setCorrectedBOLFee(Boolean correctedBOLFee) |
| `ResidentialFurnitureDelivery` | `Boolean` | Optional | Indicates whether shipment is a residential furniture delivery.  Defaults to false if not submitted.<br><br>**Default**: `false` | Boolean getResidentialFurnitureDelivery() | setResidentialFurnitureDelivery(Boolean residentialFurnitureDelivery) |
| `TarpingSurcharge` | `Boolean` | Optional | Indicates whether a tarping surcharge is applicable to shipment.  Defaults to false if not submitted.<br><br>**Default**: `false` | Boolean getTarpingSurcharge() | setTarpingSurcharge(Boolean tarpingSurcharge) |
| `DeliverOnlyToShipAddress` | `Boolean` | Optional | Indicates that the shipment should only be delivered to the ship address and not be a dirverted to an alternate location.<br><br>**Default**: `false` | Boolean getDeliverOnlyToShipAddress() | setDeliverOnlyToShipAddress(Boolean deliverOnlyToShipAddress) |
| `DeliverOnlyToAddressee` | `Boolean` | Optional | Indicates that the shipment should only be delivered to the addressee.<br><br>**Default**: `false` | Boolean getDeliverOnlyToAddressee() | setDeliverOnlyToAddressee(Boolean deliverOnlyToAddressee) |
| `DryIceForMedicalUse` | `Boolean` | Optional | Indicates Dry Ice in shipment for medical purposes.<br><br>**Default**: `false` | Boolean getDryIceForMedicalUse() | setDryIceForMedicalUse(Boolean dryIceForMedicalUse) |
| `CarbonNeutral` | `Boolean` | Optional | Indicates that the shipment should delivered in a carbon neutral manner.<br><br>**Default**: `false` | Boolean getCarbonNeutral() | setCarbonNeutral(Boolean carbonNeutral) |
| `ShipmentRequisitionID` | `Integer` | Optional | Shipment Requisition the shipment is to ship.<br><br>**Default**: `0` | Integer getShipmentRequisitionID() | setShipmentRequisitionID(Integer shipmentRequisitionID) |
| `PendingID` | `Integer` | Optional | Pending item the shipment is to ship.<br><br>**Default**: `0` | Integer getPendingID() | setPendingID(Integer pendingID) |
| `TotalCharge` | `Double` | Optional | Cost that the customer will be charged for the shipment.<br><br>**Default**: `0d` | Double getTotalCharge() | setTotalCharge(Double totalCharge) |
| `CustomerID` | `Integer` | Optional | Customer of the shipment.<br><br>**Default**: `0` | Integer getCustomerID() | setCustomerID(Integer customerID) |
| `CustomerDUNS` | `String` | Optional | Dun and Bradstreet (DUNS) identifier of the customer. | String getCustomerDUNS() | setCustomerDUNS(String customerDUNS) |
| `CustomerVendorNumber` | `String` | Optional | Vendor number the customer has assigned to the shipment sender. | String getCustomerVendorNumber() | setCustomerVendorNumber(String customerVendorNumber) |
| `CustomerLocationIdentifier` | `String` | Optional | Location, e.g. warehouse number, to which the shipment is destined. | String getCustomerLocationIdentifier() | setCustomerLocationIdentifier(String customerLocationIdentifier) |
| `PickupLocationIdentifier` | [`PickupLocationIdentifierEnum`](../../doc/models/pickup-location-identifier-enum.md) | Optional | Building location of the pickup | PickupLocationIdentifierEnum getPickupLocationIdentifier() | setPickupLocationIdentifier(PickupLocationIdentifierEnum pickupLocationIdentifier) |
| `AccountID` | `Integer` | Optional | The account identifier that identifies the carrier account to use when shipping.<br><br>**Default**: `0` | Integer getAccountID() | setAccountID(Integer accountID) |
| `ShippingKeyID` | `Integer` | Optional | Shipping key identifier override when using consolidated shipping.<br><br>**Default**: `0` | Integer getShippingKeyID() | setShippingKeyID(Integer shippingKeyID) |
| `CarrierName` | `String` | Optional | The name for the carrier. | String getCarrierName() | setCarrierName(String carrierName) |
| `TruckSize` | `String` | Optional | Size of the truck need to carry the shipment. | String getTruckSize() | setTruckSize(String truckSize) |
| `RouteID` | `Integer` | Optional | Route recommended for the shipment by the routing process.<br><br>**Default**: `0` | Integer getRouteID() | setRouteID(Integer routeID) |
| `RouteCode` | `String` | Optional | Carrier specific routing code for the shipment.<br><br>**Default**: `"0"` | String getRouteCode() | setRouteCode(String routeCode) |
| `RequiresASN` | `Boolean` | Optional | Indicates whether the shipment requires an Advance Ship Notice (ASN).  Defaults to not required if not submitted.<br><br>**Default**: `false` | Boolean getRequiresASN() | setRequiresASN(Boolean requiresASN) |
| `ShipmentDescription` | `String` | Optional | Description of the shipment's contents.  May be printed on the shipping label (dependent on which Carrier is used). | String getShipmentDescription() | setShipmentDescription(String shipmentDescription) |
| `Security` | `Boolean` | Optional | Indicates whether the shipment requires a security fee.<br><br>**Default**: `false` | Boolean getSecurity() | setSecurity(Boolean security) |
| `PriorDeliveryNotification` | `Boolean` | Optional | Indicates whether the shipment requires a prior delivery notification.<br><br>**Default**: `false` | Boolean getPriorDeliveryNotification() | setPriorDeliveryNotification(Boolean priorDeliveryNotification) |
| `Unpack` | `Boolean` | Optional | Indicates whether the shipment requires an unpack delivery fee.<br><br>**Default**: `false` | Boolean getUnpack() | setUnpack(Boolean unpack) |
| `HealthInsurance` | `Boolean` | Optional | Indicates whether the shipment requires the package requires a Health Insurance fee.<br><br>**Default**: `false` | Boolean getHealthInsurance() | setHealthInsurance(Boolean healthInsurance) |
| `SpecialDelivery` | `Boolean` | Optional | Indicates whether the shipment requires a special delivery fee.<br><br>**Default**: `false` | Boolean getSpecialDelivery() | setSpecialDelivery(Boolean specialDelivery) |
| `ForkliftDelivery` | `Boolean` | Optional | Indicates whether the shipment requires a forklift delivery fee.<br><br>**Default**: `false` | Boolean getForkliftDelivery() | setForkliftDelivery(Boolean forkliftDelivery) |
| `InsidePickup` | `Boolean` | Optional | Indicates whether the shipment is to be picked up inside.  Defaults to not inside pickup if omitted.<br><br>**Default**: `false` | Boolean getInsidePickup() | setInsidePickup(Boolean insidePickup) |
| `InsideDelivery` | `Boolean` | Optional | Indicates whether the shipment is to be delivered inside.  Defaults to not inside delivery if omitted.<br><br>**Default**: `false` | Boolean getInsideDelivery() | setInsideDelivery(Boolean insideDelivery) |
| `DoNotBreakDown` | `Boolean` | Optional | Indicates whether the shipment pallets should not be broken down.<br><br>**Default**: `false` | Boolean getDoNotBreakDown() | setDoNotBreakDown(Boolean doNotBreakDown) |
| `DoNotStackPallets` | `Boolean` | Optional | Indicates whether the shipment pallets should not be stacked.<br><br>**Default**: `false` | Boolean getDoNotStackPallets() | setDoNotStackPallets(Boolean doNotStackPallets) |
| `Oversized` | `Boolean` | Optional | Indicates whether the shipment is over-sized or of extreme length.<br><br>**Default**: `false` | Boolean getOversized() | setOversized(Boolean oversized) |
| `TopLoadOnly` | `Boolean` | Optional | Freight specific top loading only.<br><br>**Default**: `false` | Boolean getTopLoadOnly() | setTopLoadOnly(Boolean topLoadOnly) |
| `Food` | `Boolean` | Optional | Indicates whether the shipment contains food produce.<br><br>**Default**: `false` | Boolean getFood() | setFood(Boolean food) |
| `Poison` | `Boolean` | Optional | Indicates whether the shipment contains poisonous goods.<br><br>**Default**: `false` | Boolean getPoison() | setPoison(Boolean poison) |
| `DefaultWeightUOM` | `String` | Optional | Default weight units of measure for the transaction. | String getDefaultWeightUOM() | setDefaultWeightUOM(String defaultWeightUOM) |
| `DefaultDimensionsUOM` | `String` | Optional | Default dimensions units of measure for the transaction. | String getDefaultDimensionsUOM() | setDefaultDimensionsUOM(String defaultDimensionsUOM) |
| `DefaultCurrency` | `String` | Optional | Default currency for the transaction. | String getDefaultCurrency() | setDefaultCurrency(String defaultCurrency) |
| `ConsolidatedShipmentID` | `Integer` | Optional | The identifier of the consolidated shipment.<br><br>**Default**: `0` | Integer getConsolidatedShipmentID() | setConsolidatedShipmentID(Integer consolidatedShipmentID) |
| `ConsolidatedShipmentTypeID` | `Integer` | Optional | The type of the consolidated shipment.<br><br>**Default**: `0` | Integer getConsolidatedShipmentTypeID() | setConsolidatedShipmentTypeID(Integer consolidatedShipmentTypeID) |
| `ShipmentIdentifier` | `String` | Optional | Allows the internal Shipment Identifier to be overridden in a ship request to that of a user supplied value. | String getShipmentIdentifier() | setShipmentIdentifier(String shipmentIdentifier) |
| `QuickRate` | `Boolean` | Optional | Indicates whether the quote can be used for shipment or not.<br><br>**Default**: `false` | Boolean getQuickRate() | setQuickRate(Boolean quickRate) |
| `Truckload` | `Boolean` | Optional | Indicates whether this is a truckload shipment.  Defaults to not truckload if not submitted.<br><br>**Default**: `false` | Boolean getTruckload() | setTruckload(Boolean truckload) |
| `FreightAllKinds` | `Boolean` | Optional | Indicates whether to return FAK carriers.  Defaults to do not return FAK carriers if not submitted.<br><br>**Default**: `false` | Boolean getFreightAllKinds() | setFreightAllKinds(Boolean freightAllKinds) |
| `Interline` | `Boolean` | Optional | Indicates whether to return interline carriers.  Defaults to do not return interline carriers if not submitted.<br><br>**Default**: `false` | Boolean getInterline() | setInterline(Boolean interline) |
| `AccessorialCodes` | `String` | Optional | Accessorial codes that apply to the shipment. | String getAccessorialCodes() | setAccessorialCodes(String accessorialCodes) |
| `LoadingDockDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to has a loading dock.  Defaults to no loading dock if not submitted.<br><br>**Default**: `false` | Boolean getLoadingDockDelivery() | setLoadingDockDelivery(Boolean loadingDockDelivery) |
| `ConstructionSitePickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a construction site. Defaults to 'not a construction site' if not submitted.<br><br>**Default**: `false` | Boolean getConstructionSitePickup() | setConstructionSitePickup(Boolean constructionSitePickup) |
| `ConstructionSiteDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a construction site. Defaults to 'not a construction site' if not submitted.<br><br>**Default**: `false` | Boolean getConstructionSiteDelivery() | setConstructionSiteDelivery(Boolean constructionSiteDelivery) |
| `TradeShowPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a trade show. Defaults to 'not a trade show' if not submitted.<br><br>**Default**: `false` | Boolean getTradeShowPickup() | setTradeShowPickup(Boolean tradeShowPickup) |
| `TradeShowDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a trade show. Defaults to 'not a trade show' if not submitted.<br><br>**Default**: `false` | Boolean getTradeShowDelivery() | setTradeShowDelivery(Boolean tradeShowDelivery) |
| `LiftGateDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to requires a lift gate.  Defaults to no lift gate required if not submitted.<br><br>**Default**: `false` | Boolean getLiftGateDelivery() | setLiftGateDelivery(Boolean liftGateDelivery) |
| `LiftGatePickup` | `Boolean` | Optional | Indicates whether the address to be picked up from requires a lift gate.  Defaults to no lift gate required if not submitted.<br><br>**Default**: `false` | Boolean getLiftGatePickup() | setLiftGatePickup(Boolean liftGatePickup) |
| `AppointmentDelivery` | `Boolean` | Optional | Indicates whether an appointment must be made prior to delivery.  Defaults to no appointment needed if not submitted.<br><br>**Default**: `false` | Boolean getAppointmentDelivery() | setAppointmentDelivery(Boolean appointmentDelivery) |
| `AppointmentPickup` | `Boolean` | Optional | Indicates whether an appointment must be made prior to pick up.  Defaults to no appointment needed if not submitted.<br><br>**Default**: `false` | Boolean getAppointmentPickup() | setAppointmentPickup(Boolean appointmentPickup) |
| `NineAMDelivery` | `Boolean` | Optional | Indicates whether a shipment should be delivered before 9AM.<br><br>**Default**: `false` | Boolean getNineAMDelivery() | setNineAMDelivery(Boolean nineAMDelivery) |
| `DeliveryWindow` | `Boolean` | Optional | Indicates whether a delivery window has been specified for this shipment.<br><br>**Default**: `false` | Boolean getDeliveryWindow() | setDeliveryWindow(Boolean deliveryWindow) |
| `DeliverToDoor` | `Boolean` | Optional | Indicates whether the package should be delivered to door.<br><br>**Default**: `false` | Boolean getDeliverToDoor() | setDeliverToDoor(Boolean deliverToDoor) |
| `DeliveryWindowAfterDate` | `String` | Optional | Indicates the date from which the shipment can be delivered. | String getDeliveryWindowAfterDate() | setDeliveryWindowAfterDate(String deliveryWindowAfterDate) |
| `DeliveryWindowAfterTime` | `String` | Optional | Indicates the time from which the shipment can be delivered. | String getDeliveryWindowAfterTime() | setDeliveryWindowAfterTime(String deliveryWindowAfterTime) |
| `DeliveryWindowBeforeDate` | `String` | Optional | Indicates the date after which the shipment should not be delivered. | String getDeliveryWindowBeforeDate() | setDeliveryWindowBeforeDate(String deliveryWindowBeforeDate) |
| `DeliveryWindowBeforeTime` | `String` | Optional | Indicates the time after which the shipment should not be delivered. | String getDeliveryWindowBeforeTime() | setDeliveryWindowBeforeTime(String deliveryWindowBeforeTime) |
| `AuthorizationID` | `String` | Optional | Authorization ID for an associated special service. | String getAuthorizationID() | setAuthorizationID(String authorizationID) |
| `UnloadFreightAtDelivery` | `Boolean` | Optional | Indicates whether the shipment requires unloading on delivery.  Defaults to unloading not required if not submitted.<br><br>**Default**: `false` | Boolean getUnloadFreightAtDelivery() | setUnloadFreightAtDelivery(Boolean unloadFreightAtDelivery) |
| `LoadFreightAtPickup` | `Boolean` | Optional | Indicates whether the shipment requires loading on pick up.  Defaults to loading not required if not submitted.<br><br>**Default**: `false` | Boolean getLoadFreightAtPickup() | setLoadFreightAtPickup(Boolean loadFreightAtPickup) |
| `WhiteGlove` | `Boolean` | Optional | Indicates whether the shipment requires white glove handling.  Defaults to white glove handling not required if not submitted.<br><br>**Default**: `false` | Boolean getWhiteGlove() | setWhiteGlove(Boolean whiteGlove) |
| `TwoManDelivery` | `Boolean` | Optional | Indicates whether the shipment requires a two man delivery.  Defaults to two man delivery not required if not submitted.<br><br>**Default**: `false` | Boolean getTwoManDelivery() | setTwoManDelivery(Boolean twoManDelivery) |
| `PalletExchange` | `Boolean` | Optional | Indicates whether the shipment requires pallet exchange.  Defaults to pallet exchange not required if not submitted.<br><br>**Default**: `false` | Boolean getPalletExchange() | setPalletExchange(Boolean palletExchange) |
| `SortAndSegregate` | `Boolean` | Optional | Indicates whether the shipment requires sorting and segregating.  Defaults to sorting and segregating not required if not submitted.<br><br>**Default**: `false` | Boolean getSortAndSegregate() | setSortAndSegregate(Boolean sortAndSegregate) |
| `Wholesaler` | `Boolean` | Optional | Indicates whether the shipment requires wholesaling.  Defaults to Wholesaling not required if not submitted.<br><br>**Default**: `false` | Boolean getWholesaler() | setWholesaler(Boolean wholesaler) |
| `TobaccoReportingCharge` | `Boolean` | Optional | Indicates whether the shipment requires tobacco reporting charge.  Defaults to tobacco reporting charge not required if not submitted.<br><br>**Default**: `false` | Boolean getTobaccoReportingCharge() | setTobaccoReportingCharge(Boolean tobaccoReportingCharge) |
| `Bulkhead` | `Boolean` | Optional | Indicates whether the shipment requires bulkhead.  Defaults to bulkhead not required if not submitted.<br><br>**Default**: `false` | Boolean getBulkhead() | setBulkhead(Boolean bulkhead) |
| `CallBeforeDelivery` | `Boolean` | Optional | Indicates whether the shipment requires call before delivery, arrival notice, notify charge.  Defaults to call before delivery not required if not submitted.<br><br>**Default**: `false` | Boolean getCallBeforeDelivery() | setCallBeforeDelivery(Boolean callBeforeDelivery) |
| `HighCostDeliverySurcharge` | `Boolean` | Optional | Indicates whether the shipment requires high cost delivery surcharge.  Defaults to high cost delivery surcharge not required if not submitted.<br><br>**Default**: `false` | Boolean getHighCostDeliverySurcharge() | setHighCostDeliverySurcharge(Boolean highCostDeliverySurcharge) |
| `LimitedAccessDelivery` | `Boolean` | Optional | Indicates whether the shipment requires limited access delivery charge.  Defaults to limited access delivery charge not required if not submitted.<br><br>**Default**: `false` | Boolean getLimitedAccessDelivery() | setLimitedAccessDelivery(Boolean limitedAccessDelivery) |
| `RemoteLocationSurcharge` | `Boolean` | Optional | Indicates whether the shipment requires remote location surcharge.  Defaults to remote location surcharge not required if not submitted.<br><br>**Default**: `false` | Boolean getRemoteLocationSurcharge() | setRemoteLocationSurcharge(Boolean remoteLocationSurcharge) |
| `AMDelivery` | `Boolean` | Optional | Indicates whether the shipment is an AM Delivery.  Defaults to false if not submitted.<br><br>**Default**: `false` | Boolean getAMDelivery() | setAMDelivery(Boolean aMDelivery) |
| `SingleShipment` | `Boolean` | Optional | Indicates whether the shipment is a single shipment.  Defaults to false if not submitted.<br><br>**Default**: `false` | Boolean getSingleShipment() | setSingleShipment(Boolean singleShipment) |
| `LimitedAccessPickup` | `Boolean` | Optional | Indicates whether the shipment is to be picked up from a location with limited access.  Defaults to false if not submitted.<br><br>**Default**: `false` | Boolean getLimitedAccessPickup() | setLimitedAccessPickup(Boolean limitedAccessPickup) |
| `AirportPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a airport. Defaults to 'not a airport' if not submitted.<br><br>**Default**: `false` | Boolean getAirportPickup() | setAirportPickup(Boolean airportPickup) |
| `CampPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a camp. Defaults to 'not a camp' if not submitted.<br><br>**Default**: `false` | Boolean getCampPickup() | setCampPickup(Boolean campPickup) |
| `CertifiedPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is certified. Defaults to 'not certified' if not submitted.<br><br>**Default**: `false` | Boolean getCertifiedPickup() | setCertifiedPickup(Boolean certifiedPickup) |
| `ChurchPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a church. Defaults to 'not a church' if not submitted.<br><br>**Default**: `false` | Boolean getChurchPickup() | setChurchPickup(Boolean churchPickup) |
| `CountryClubPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a country club. Defaults to 'not a country club' if not submitted.<br><br>**Default**: `false` | Boolean getCountryClubPickup() | setCountryClubPickup(Boolean countryClubPickup) |
| `CommercialPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a commercial pickup. Defaults to 'not a commercial pickup' if not submitted.<br><br>**Default**: `false` | Boolean getCommercialPickup() | setCommercialPickup(Boolean commercialPickup) |
| `DockPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a dock. Defaults to 'not a dock' if not submitted.<br><br>**Default**: `false` | Boolean getDockPickup() | setDockPickup(Boolean dockPickup) |
| `DeclaredValuePickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a declared value pickup. Defaults to 'not a declared value pickup' if not submitted.<br><br>**Default**: `false` | Boolean getDeclaredValuePickup() | setDeclaredValuePickup(Boolean declaredValuePickup) |
| `SchoolPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a school. Defaults to 'not a school' if not submitted.<br><br>**Default**: `false` | Boolean getSchoolPickup() | setSchoolPickup(Boolean schoolPickup) |
| `FarmPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a farm. Defaults to 'not a farm' if not submitted.<br><br>**Default**: `false` | Boolean getFarmPickup() | setFarmPickup(Boolean farmPickup) |
| `FlatbedPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a flat bed pickup. Defaults to 'not a flat bed pickup' if not submitted.<br><br>**Default**: `false` | Boolean getFlatbedPickup() | setFlatbedPickup(Boolean flatbedPickup) |
| `GovernmentSitePickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a government site. Defaults to 'not a government site' if not submitted.<br><br>**Default**: `false` | Boolean getGovernmentSitePickup() | setGovernmentSitePickup(Boolean governmentSitePickup) |
| `GroceryWarehousePickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a grocery warehouse. Defaults to 'not a grovery warehouse' if not submitted.<br><br>**Default**: `false` | Boolean getGroceryWarehousePickup() | setGroceryWarehousePickup(Boolean groceryWarehousePickup) |
| `HospitalPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a hospital. Defaults to 'not a hospital' if not submitted.<br><br>**Default**: `false` | Boolean getHospitalPickup() | setHospitalPickup(Boolean hospitalPickup) |
| `HotelPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a hotel. Defaults to 'not a hotel' if not submitted.<br><br>**Default**: `false` | Boolean getHotelPickup() | setHotelPickup(Boolean hotelPickup) |
| `MallPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a mail pickup. Defaults to 'not a mail pickup' if not submitted.<br><br>**Default**: `false` | Boolean getMallPickup() | setMallPickup(Boolean mallPickup) |
| `MilitaryInstallationPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a military installation. Defaults to 'not a military installation' if not submitted.<br><br>**Default**: `false` | Boolean getMilitaryInstallationPickup() | setMilitaryInstallationPickup(Boolean militaryInstallationPickup) |
| `MineSitePickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a mine. Defaults to 'not a mine' if not submitted.<br><br>**Default**: `false` | Boolean getMineSitePickup() | setMineSitePickup(Boolean mineSitePickup) |
| `NativeAmericanReservationPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a native american reservation. Defaults to 'not a native american reservation' if not submitted.<br><br>**Default**: `false` | Boolean getNativeAmericanReservationPickup() | setNativeAmericanReservationPickup(Boolean nativeAmericanReservationPickup) |
| `NonBusinessHoursPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a non business hours pickup. Defaults to 'not a non business hours pickup' if not submitted.<br><br>**Default**: `false` | Boolean getNonBusinessHoursPickup() | setNonBusinessHoursPickup(Boolean nonBusinessHoursPickup) |
| `NonCommercialPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a non commercial pickup. Defaults to 'not a non commercial pickup' if not submitted.<br><br>**Default**: `false` | Boolean getNonCommercialPickup() | setNonCommercialPickup(Boolean nonCommercialPickup) |
| `NursingHomePickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a nursing home. Defaults to 'not a nursing home' if not submitted.<br><br>**Default**: `false` | Boolean getNursingHomePickup() | setNursingHomePickup(Boolean nursingHomePickup) |
| `OversizedPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a oversized pickup. Defaults to 'not a oversized pickup' if not submitted.<br><br>**Default**: `false` | Boolean getOversizedPickup() | setOversizedPickup(Boolean oversizedPickup) |
| `FairAmusementParkPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a fair, amusements or park. Defaults to 'not a fair, amusements or park' if not submitted.<br><br>**Default**: `false` | Boolean getFairAmusementParkPickup() | setFairAmusementParkPickup(Boolean fairAmusementParkPickup) |
| `PierPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a pier. Defaults to 'not a pier' if not submitted.<br><br>**Default**: `false` | Boolean getPierPickup() | setPierPickup(Boolean pierPickup) |
| `PalletJackPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a pallet jack pickup. Defaults to 'not a pallet jack pickup' if not submitted.<br><br>**Default**: `false` | Boolean getPalletJackPickup() | setPalletJackPickup(Boolean palletJackPickup) |
| `PrisonPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a prison. Defaults to 'not a prison' if not submitted.<br><br>**Default**: `false` | Boolean getPrisonPickup() | setPrisonPickup(Boolean prisonPickup) |
| `ResortPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a resort. Defaults to 'not a resort' if not submitted.<br><br>**Default**: `false` | Boolean getResortPickup() | setResortPickup(Boolean resortPickup) |
| `SortSegregatePickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a sort segregate pickup. Defaults to 'not a sort segregate pickup' if not submitted.<br><br>**Default**: `false` | Boolean getSortSegregatePickup() | setSortSegregatePickup(Boolean sortSegregatePickup) |
| `SelfStoragePickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a self storage pickup. Defaults to 'not a self storage pickup' if not submitted.<br><br>**Default**: `false` | Boolean getSelfStoragePickup() | setSelfStoragePickup(Boolean selfStoragePickup) |
| `UtilitySitePickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a utility site. Defaults to 'not a utility site' if not submitted.<br><br>**Default**: `false` | Boolean getUtilitySitePickup() | setUtilitySitePickup(Boolean utilitySitePickup) |
| `PalletExchangePickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a pallet exchange pickup. Defaults to 'not a pallet exchange pickup' if not submitted.<br><br>**Default**: `false` | Boolean getPalletExchangePickup() | setPalletExchangePickup(Boolean palletExchangePickup) |
| `DockTransferPickup` | `Boolean` | Optional | Indicates whether the address to be picked up from to is a dock transfer pickup. Defaults to 'not a dock transfer pickup' if not submitted.<br><br>**Default**: `false` | Boolean getDockTransferPickup() | setDockTransferPickup(Boolean dockTransferPickup) |
| `AirportDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is an airport. Defaults to 'not an airport' if not submitted.<br><br>**Default**: `false` | Boolean getAirportDelivery() | setAirportDelivery(Boolean airportDelivery) |
| `AdvancedCollection` | `Boolean` | Optional | Indicates whether the delivery is an advanced delivery. Defaults to 'not an AdvancedCollection' if not submitted.<br><br>**Default**: `false` | Boolean getAdvancedCollection() | setAdvancedCollection(Boolean advancedCollection) |
| `CampDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a camp. Defaults to 'not a camp' if not submitted.<br><br>**Default**: `false` | Boolean getCampDelivery() | setCampDelivery(Boolean campDelivery) |
| `ChurchDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a church. Defaults to 'not a church' if not submitted.<br><br>**Default**: `false` | Boolean getChurchDelivery() | setChurchDelivery(Boolean churchDelivery) |
| `CountryClubDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a country club. Defaults to 'not a country club' if not submitted.<br><br>**Default**: `false` | Boolean getCountryClubDelivery() | setCountryClubDelivery(Boolean countryClubDelivery) |
| `CommercialDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is commercial. Defaults to 'not commercial' if not submitted.<br><br>**Default**: `false` | Boolean getCommercialDelivery() | setCommercialDelivery(Boolean commercialDelivery) |
| `DistributionCenterDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a distribution center. Defaults to 'not a distribution center' if not submitted.<br><br>**Default**: `false` | Boolean getDistributionCenterDelivery() | setDistributionCenterDelivery(Boolean distributionCenterDelivery) |
| `DeclaredValueDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a declared value delivery. Defaults to 'not a declared value delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDeclaredValueDelivery() | setDeclaredValueDelivery(Boolean declaredValueDelivery) |
| `SchoolDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a school. Defaults to 'not a school' if not submitted.<br><br>**Default**: `false` | Boolean getSchoolDelivery() | setSchoolDelivery(Boolean schoolDelivery) |
| `EmergencyDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is an emergency delivery. Defaults to 'not an emergency delivery' if not submitted.<br><br>**Default**: `false` | Boolean getEmergencyDelivery() | setEmergencyDelivery(Boolean emergencyDelivery) |
| `FarmDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a farm. Defaults to 'not a farm' if not submitted.<br><br>**Default**: `false` | Boolean getFarmDelivery() | setFarmDelivery(Boolean farmDelivery) |
| `FlatbedDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a flat bed delivery. Defaults to 'not a flat bed delivery' if not submitted.<br><br>**Default**: `false` | Boolean getFlatbedDelivery() | setFlatbedDelivery(Boolean flatbedDelivery) |
| `GovernmentSiteDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a government site. Defaults to 'not a government site' if not submitted.<br><br>**Default**: `false` | Boolean getGovernmentSiteDelivery() | setGovernmentSiteDelivery(Boolean governmentSiteDelivery) |
| `GroceryWarehouseDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a grocery warehouse. Defaults to 'not a grocery warehouse' if not submitted.<br><br>**Default**: `false` | Boolean getGroceryWarehouseDelivery() | setGroceryWarehouseDelivery(Boolean groceryWarehouseDelivery) |
| `HospitalDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a hospital. Defaults to 'not a hospital' if not submitted.<br><br>**Default**: `false` | Boolean getHospitalDelivery() | setHospitalDelivery(Boolean hospitalDelivery) |
| `HotelDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a hotel. Defaults to 'not a hotel' if not submitted.<br><br>**Default**: `false` | Boolean getHotelDelivery() | setHotelDelivery(Boolean hotelDelivery) |
| `MallDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a mall. Defaults to 'not a mall' if not submitted.<br><br>**Default**: `false` | Boolean getMallDelivery() | setMallDelivery(Boolean mallDelivery) |
| `MilitaryInstallationDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a military installation site. Defaults to 'not a military installation site' if not submitted.<br><br>**Default**: `false` | Boolean getMilitaryInstallationDelivery() | setMilitaryInstallationDelivery(Boolean militaryInstallationDelivery) |
| `MineSiteDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a mine site. Defaults to 'not a mine site' if not submitted.<br><br>**Default**: `false` | Boolean getMineSiteDelivery() | setMineSiteDelivery(Boolean mineSiteDelivery) |
| `NativeAmericanReservationDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a native american reservation. Defaults to 'not a native american reservation' if not submitted.<br><br>**Default**: `false` | Boolean getNativeAmericanReservationDelivery() | setNativeAmericanReservationDelivery(Boolean nativeAmericanReservationDelivery) |
| `NonBusinessHoursDelivery` | `Boolean` | Optional | Indicates whether the delivery will be outside of business hours. Defaults to 'inside business hours' if not submitted.<br><br>**Default**: `false` | Boolean getNonBusinessHoursDelivery() | setNonBusinessHoursDelivery(Boolean nonBusinessHoursDelivery) |
| `NonCommercialDelivery` | `Boolean` | Optional | Indicates whether the delivery is not commercial. Defaults to 'commercial' if not submitted.<br><br>**Default**: `false` | Boolean getNonCommercialDelivery() | setNonCommercialDelivery(Boolean nonCommercialDelivery) |
| `NursingHomeDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a nursing home. Defaults to 'not a nursing home' if not submitted.<br><br>**Default**: `false` | Boolean getNursingHomeDelivery() | setNursingHomeDelivery(Boolean nursingHomeDelivery) |
| `OversizedDelivery` | `Boolean` | Optional | Indicates whether the delivery is oversized. Defaults to 'not oversized' if not submitted.<br><br>**Default**: `false` | Boolean getOversizedDelivery() | setOversizedDelivery(Boolean oversizedDelivery) |
| `FairAmusementParkDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a fair, amusements or park. Defaults to 'not a fair, amusements or park' if not submitted.<br><br>**Default**: `false` | Boolean getFairAmusementParkDelivery() | setFairAmusementParkDelivery(Boolean fairAmusementParkDelivery) |
| `PierDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a pier. Defaults to 'not a pier' if not submitted.<br><br>**Default**: `false` | Boolean getPierDelivery() | setPierDelivery(Boolean pierDelivery) |
| `PalletJackDelivery` | `Boolean` | Optional | Indicates whether a pallet jack is required for delivery. Defaults to 'not a pallet jack is not required' if not submitted.<br><br>**Default**: `false` | Boolean getPalletJackDelivery() | setPalletJackDelivery(Boolean palletJackDelivery) |
| `PrisonDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a prison. Defaults to 'not a prison' if not submitted.<br><br>**Default**: `false` | Boolean getPrisonDelivery() | setPrisonDelivery(Boolean prisonDelivery) |
| `ResortDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a resort. Defaults to 'not a resort' if not submitted.<br><br>**Default**: `false` | Boolean getResortDelivery() | setResortDelivery(Boolean resortDelivery) |
| `SortSegregateDelivery` | `Boolean` | Optional | Indicates whether the delivery is a sort segration. Defaults to 'not a sort segration' if not submitted.<br><br>**Default**: `false` | Boolean getSortSegregateDelivery() | setSortSegregateDelivery(Boolean sortSegregateDelivery) |
| `SelfStorageDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a self storage facility. Defaults to 'not a self storage facility' if not submitted.<br><br>**Default**: `false` | Boolean getSelfStorageDelivery() | setSelfStorageDelivery(Boolean selfStorageDelivery) |
| `UtilitySiteDelivery` | `Boolean` | Optional | Indicates whether the address to be delivered to is a utility site. Defaults to 'not a utility site' if not submitted.<br><br>**Default**: `false` | Boolean getUtilitySiteDelivery() | setUtilitySiteDelivery(Boolean utilitySiteDelivery) |
| `PalletExchangeDelivery` | `Boolean` | Optional | Indicates that this is a pallet exchange delivery. Defaults to 'not a pallet exchange delivery' if not submitted.<br><br>**Default**: `false` | Boolean getPalletExchangeDelivery() | setPalletExchangeDelivery(Boolean palletExchangeDelivery) |
| `DockTransferDelivery` | `Boolean` | Optional | Indicates that this is a dock transfer delivery. Defaults to 'not a dock transfer delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDockTransferDelivery() | setDockTransferDelivery(Boolean dockTransferDelivery) |
| `InsideDeliveryType` | `Integer` | Optional | Numeric identifier for the type of inside delivery.  Defaults to no inside delivery if not submitted.<br><br>**Constraints**: *Pattern*: `[1-5]` | Integer getInsideDeliveryType() | setInsideDeliveryType(Integer insideDeliveryType) |
| `AfterHoursCharge` | `Boolean` | Optional | Indicates that this after hours charge delivery. Defaults to 'not a after hours charge delivery' if not submitted.<br><br>**Default**: `false` | Boolean getAfterHoursCharge() | setAfterHoursCharge(Boolean afterHoursCharge) |
| `AirFreight` | `Boolean` | Optional | Indicates that this is a air freight delivery. Defaults to 'not a air freight delivery' if not submitted.<br><br>**Default**: `false` | Boolean getAirFreight() | setAirFreight(Boolean airFreight) |
| `AirBag` | `Boolean` | Optional | Indicates that this is a air bag delivery. Defaults to 'not a air bag delivery' if not submitted.<br><br>**Default**: `false` | Boolean getAirBag() | setAirBag(Boolean airBag) |
| `ArbitraryCharge` | `Boolean` | Optional | Indicates that this is a arbitrary charge delivery. Defaults to 'not a arbitrary charge delivery' if not submitted.<br><br>**Default**: `false` | Boolean getArbitraryCharge() | setArbitraryCharge(Boolean arbitraryCharge) |
| `BagLiner` | `Boolean` | Optional | Indicates that this is a bag liner delivery. Defaults to 'not a bag liner delivery' if not submitted.<br><br>**Default**: `false` | Boolean getBagLiner() | setBagLiner(Boolean bagLiner) |
| `BlindShipment` | `Boolean` | Optional | Indicates that this is a blind shipment. Defaults to 'not a blind shipment' if not submitted.<br><br>**Default**: `false` | Boolean getBlindShipment() | setBlindShipment(Boolean blindShipment) |
| `Bobtail` | `Boolean` | Optional | Indicates that this is a bobtail delivery. Defaults to 'not a bobtail delivery' if not submitted.<br><br>**Default**: `false` | Boolean getBobtail() | setBobtail(Boolean bobtail) |
| `InBondShipment` | `Boolean` | Optional | Indicates that this is a in bond shipment delivery. Defaults to 'not a in bond shipment delivery' if not submitted.<br><br>**Default**: `false` | Boolean getInBondShipment() | setInBondShipment(Boolean inBondShipment) |
| `BeyondIndirectService` | `Boolean` | Optional | Indicates that this is a beyond indirect service delivery. Defaults to 'not a beyond indirect service delivery' if not submitted.<br><br>**Default**: `false` | Boolean getBeyondIndirectService() | setBeyondIndirectService(Boolean beyondIndirectService) |
| `NorthboundCanadianBorderCrossingDocumentHandlingFee` | `Boolean` | Optional | Indicates that this is a northbound canadian border crossing document handling fee delivery. Defaults to 'not a northbound canadian border crossing document handling fee delivery' if not submitted.<br><br>**Default**: `false` | Boolean getNorthboundCanadianBorderCrossingDocumentHandlingFee() | setNorthboundCanadianBorderCrossingDocumentHandlingFee(Boolean northboundCanadianBorderCrossingDocumentHandlingFee) |
| `CapacityLoadPup` | `Boolean` | Optional | Indicates that this is a capacity load pup delivery. Defaults to 'not a capacity load pup delivery' if not submitted.<br><br>**Default**: `false` | Boolean getCapacityLoadPup() | setCapacityLoadPup(Boolean capacityLoadPup) |
| `CapacityLoadTrailer` | `Boolean` | Optional | Indicates that this is a capacity load trailer. Defaults to 'not a capacity load trailer delivery' if not submitted.<br><br>**Default**: `false` | Boolean getCapacityLoadTrailer() | setCapacityLoadTrailer(Boolean capacityLoadTrailer) |
| `ChassisTruck` | `Boolean` | Optional | Indicates that this is a chassis truck delivery. Defaults to 'not a chassis truck delivery' if not submitted.<br><br>**Default**: `false` | Boolean getChassisTruck() | setChassisTruck(Boolean chassisTruck) |
| `ChangeofBOL` | `Boolean` | Optional | Indicates that this is a change of BOL delivery. Defaults to 'not a change of BOL delivery' if not submitted.<br><br>**Default**: `false` | Boolean getChangeofBOL() | setChangeofBOL(Boolean changeofBOL) |
| `Consolidation` | `Boolean` | Optional | Indicates that this is a consolidation delivery. Defaults to 'not a consolidation delivery' if not submitted.<br><br>**Default**: `false` | Boolean getConsolidation() | setConsolidation(Boolean consolidation) |
| `CorrectedBOL` | `Boolean` | Optional | Indicates that this is a corrected BOL delivery. Defaults to 'not a corrected BOL delivery' if not submitted.<br><br>**Default**: `false` | Boolean getCorrectedBOL() | setCorrectedBOL(Boolean correctedBOL) |
| `CranePermits` | `Boolean` | Optional | Indicates that this is a crane permits delivery. Defaults to 'not a crane permits delivery' if not submitted.<br><br>**Default**: `false` | Boolean getCranePermits() | setCranePermits(Boolean cranePermits) |
| `RedelivertoConsignee` | `Boolean` | Optional | Indicates that this is a redeliver to consignee delivery. Defaults to 'not a redeliver to consignee delivery' if not submitted.<br><br>**Default**: `false` | Boolean getRedelivertoConsignee() | setRedelivertoConsignee(Boolean redelivertoConsignee) |
| `CrossDock` | `Boolean` | Optional | Indicates that this is a cross dock delivery. Defaults to 'not a cross dock delivery' if not submitted.<br><br>**Default**: `false` | Boolean getCrossDock() | setCrossDock(Boolean crossDock) |
| `DescriptionInspection` | `Boolean` | Optional | Indicates that this is a description inspection delivery. Defaults to 'not a description inspection delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDescriptionInspection() | setDescriptionInspection(Boolean descriptionInspection) |
| `Detention` | `Boolean` | Optional | Indicates that this is a detention delivery. Defaults to 'not a detention delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDetention() | setDetention(Boolean detention) |
| `DelayCharge` | `Boolean` | Optional | Indicates that this is a delay charge delivery. Defaults to 'not a delay charge delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDelayCharge() | setDelayCharge(Boolean delayCharge) |
| `DriverAssistance` | `Boolean` | Optional | Indicates that this is a driver assistance delivery. Defaults to 'not a driver assistance delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDriverAssistance() | setDriverAssistance(Boolean driverAssistance) |
| `Drayage` | `Boolean` | Optional | Indicates that this is a drayage delivery. Defaults to 'not a drayage delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDrayage() | setDrayage(Boolean drayage) |
| `DropPull` | `Boolean` | Optional | Indicates that this is a drop pull delivery. Defaults to 'not a drop pull delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDropPull() | setDropPull(Boolean dropPull) |
| `DryRun` | `Boolean` | Optional | Indicates that this is a dry run delivery. Defaults to 'not a dry run delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDryRun() | setDryRun(Boolean dryRun) |
| `Excessivevalue` | `Boolean` | Optional | Indicates that this delivery has an excessive value. Defaults to 'not an excessive value' if not submitted.<br><br>**Default**: `false` | Boolean getExcessivevalue() | setExcessivevalue(Boolean excessivevalue) |
| `ExportShipment` | `Boolean` | Optional | Indicates that this is a export shipment delivery. Defaults to 'not a export shipment delivery' if not submitted.<br><br>**Default**: `false` | Boolean getExportShipment() | setExportShipment(Boolean exportShipment) |
| `FlatTrack` | `Boolean` | Optional | Indicates that this is a flat track delivery. Defaults to 'not a flat track delivery' if not submitted.<br><br>**Default**: `false` | Boolean getFlatTrack() | setFlatTrack(Boolean flatTrack) |
| `ShipmentContainsFood` | `Boolean` | Optional | Indicates that this is delivery contains food. Defaults to 'delivery does not contain food' if not submitted.<br><br>**Default**: `false` | Boolean getShipmentContainsFood() | setShipmentContainsFood(Boolean shipmentContainsFood) |
| `Forklift` | `Boolean` | Optional | Indicates that this is a fork lift delivery. Defaults to 'not a fork lift delivery' if not submitted.<br><br>**Default**: `false` | Boolean getForklift() | setForklift(Boolean forklift) |
| `HawaiianWillCall` | `Boolean` | Optional | Indicates that this is a Hawaiian will call delivery. Defaults to 'not a Hawaiian will call delivery' if not submitted.<br><br>**Default**: `false` | Boolean getHawaiianWillCall() | setHawaiianWillCall(Boolean hawaiianWillCall) |
| `HighDockEquipmentNeeded` | `Boolean` | Optional | Indicates that this is a high dock equipment needed delivery. Defaults to 'not a high dock equipment needed delivery' if not submitted.<br><br>**Default**: `false` | Boolean getHighDockEquipmentNeeded() | setHighDockEquipmentNeeded(Boolean highDockEquipmentNeeded) |
| `HomeLandSecurity` | `Boolean` | Optional | Indicates that this is a home land security delivery. Defaults to 'not a home land security delivery' if not submitted.<br><br>**Default**: `false` | Boolean getHomeLandSecurity() | setHomeLandSecurity(Boolean homeLandSecurity) |
| `HolidayWeekendService` | `Boolean` | Optional | Indicates that this is a holiday weekend service delivery. Defaults to 'not a holiday weekend service delivery' if not submitted.<br><br>**Default**: `false` | Boolean getHolidayWeekendService() | setHolidayWeekendService(Boolean holidayWeekendService) |
| `ImportShipment` | `Boolean` | Optional | Indicates that this is a import shipment delivery. Defaults to 'not a import shipment delivery' if not submitted.<br><br>**Default**: `false` | Boolean getImportShipment() | setImportShipment(Boolean importShipment) |
| `InboundFreight` | `Boolean` | Optional | Indicates that this is a inbound freight delivery. Defaults to 'not a inbound freight delivery' if not submitted.<br><br>**Default**: `false` | Boolean getInboundFreight() | setInboundFreight(Boolean inboundFreight) |
| `InterlineShipment` | `Boolean` | Optional | Indicates that this is a interline shipment delivery. Defaults to 'not a interline shipment delivery' if not submitted.<br><br>**Default**: `false` | Boolean getInterlineShipment() | setInterlineShipment(Boolean interlineShipment) |
| `InterRegionalShipment` | `Boolean` | Optional | Indicates that this is a inter regional shipment delivery. Defaults to 'not a inter regional shipment delivery' if not submitted.<br><br>**Default**: `false` | Boolean getInterRegionalShipment() | setInterRegionalShipment(Boolean interRegionalShipment) |
| `HandlingandLabeling` | `Boolean` | Optional | Indicates that this is a handling and labeling delivery. Defaults to 'not a handling and labeling delivery' if not submitted.<br><br>**Default**: `false` | Boolean getHandlingandLabeling() | setHandlingandLabeling(Boolean handlingandLabeling) |
| `LiquorPermit` | `Boolean` | Optional | Indicates that this is a liquor permit delivery. Defaults to 'not a liquor permit delivery' if not submitted.<br><br>**Default**: `false` | Boolean getLiquorPermit() | setLiquorPermit(Boolean liquorPermit) |
| `DriverLoad` | `Boolean` | Optional | Indicates that this is a driver load delivery. Defaults to 'not a driver load delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDriverLoad() | setDriverLoad(Boolean driverLoad) |
| `DriverLoadandCount` | `Boolean` | Optional | Indicates that this is a driver load and count delivery. Defaults to 'not a driver load and count delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDriverLoadandCount() | setDriverLoadandCount(Boolean driverLoadandCount) |
| `DriverLoadUnload` | `Boolean` | Optional | Indicates that this is a driver load / unload delivery. Defaults to 'not a driver load / unload delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDriverLoadUnload() | setDriverLoadUnload(Boolean driverLoadUnload) |
| `LumperService` | `Boolean` | Optional | Indicates that this is a lumper service delivery. Defaults to 'not a lumper service delivery' if not submitted.<br><br>**Default**: `false` | Boolean getLumperService() | setLumperService(Boolean lumperService) |
| `Layover` | `Boolean` | Optional | Indicates that this is a layover delivery. Defaults to 'not a layover delivery' if not submitted.<br><br>**Default**: `false` | Boolean getLayover() | setLayover(Boolean layover) |
| `MarkingorTagging` | `Boolean` | Optional | Indicates that this is a marking or tagging delivery. Defaults to 'not a marking or tagging delivery' if not submitted.<br><br>**Default**: `false` | Boolean getMarkingorTagging() | setMarkingorTagging(Boolean markingorTagging) |
| `NotifyBeforeDelivery` | `Boolean` | Optional | Indicates that this is a notify before delivery. Defaults to 'not a notify before delivery' if not submitted.<br><br>**Default**: `false` | Boolean getNotifyBeforeDelivery() | setNotifyBeforeDelivery(Boolean notifyBeforeDelivery) |
| `Over750Under6` | `Boolean` | Optional | Indicates that this is a over 750 under 6 delivery. Defaults to 'not a over 750 under 6 delivery' if not submitted.<br><br>**Default**: `false` | Boolean getOver750Under6() | setOver750Under6(Boolean over750Under6) |
| `OilSands` | `Boolean` | Optional | Indicates that this is a oil sands delivery. Defaults to 'not a oil sands delivery' if not submitted.<br><br>**Default**: `false` | Boolean getOilSands() | setOilSands(Boolean oilSands) |
| `OpenTopTruck` | `Boolean` | Optional | Indicates that this is a open top truck delivery. Defaults to 'not a open top truck delivery' if not submitted.<br><br>**Default**: `false` | Boolean getOpenTopTruck() | setOpenTopTruck(Boolean openTopTruck) |
| `OverDimensionFreight` | `Boolean` | Optional | Indicates that this is a over dimension freight delivery. Defaults to 'not a over dimension freight delivery' if not submitted.<br><br>**Default**: `false` | Boolean getOverDimensionFreight() | setOverDimensionFreight(Boolean overDimensionFreight) |
| `Overweight` | `Boolean` | Optional | Indicates that this is a overweight delivery. Defaults to 'not a overweight delivery' if not submitted.<br><br>**Default**: `false` | Boolean getOverweight() | setOverweight(Boolean overweight) |
| `Pallet` | `Boolean` | Optional | Indicates that this is a pallet delivery. Defaults to 'not a pallet delivery' if not submitted.<br><br>**Default**: `false` | Boolean getPallet() | setPallet(Boolean pallet) |
| `ProtectFromHeat` | `Boolean` | Optional | Indicates that this is a protect from heat delivery. Defaults to 'not a protect from heat delivery' if not submitted.<br><br>**Default**: `false` | Boolean getProtectFromHeat() | setProtectFromHeat(Boolean protectFromHeat) |
| `ProtectFromFreezing` | `Boolean` | Optional | Indicates that this is a protect from freezing delivery. Defaults to 'not a protect from freezing delivery' if not submitted.<br><br>**Default**: `false` | Boolean getProtectFromFreezing() | setProtectFromFreezing(Boolean protectFromFreezing) |
| `ProtectFromFreezingCanada` | `Boolean` | Optional | Indicates that this is a protect from freezing Canada delivery. Defaults to 'not a protect from freezing Canada delivery' if not submitted.<br><br>**Default**: `false` | Boolean getProtectFromFreezingCanada() | setProtectFromFreezingCanada(Boolean protectFromFreezingCanada) |
| `Permit` | `Boolean` | Optional | Indicates that this is a permit delivery. Defaults to 'not a permit delivery' if not submitted.<br><br>**Default**: `false` | Boolean getPermit() | setPermit(Boolean permit) |
| `ProtectiveService` | `Boolean` | Optional | Indicates that this is a protective service delivery. Defaults to 'not a protective service delivery' if not submitted.<br><br>**Default**: `false` | Boolean getProtectiveService() | setProtectiveService(Boolean protectiveService) |
| `ProtectiveDrumCover` | `Boolean` | Optional | Indicates that this is a protective drum cover delivery. Defaults to 'not a protective drum cover delivery' if not submitted.<br><br>**Default**: `false` | Boolean getProtectiveDrumCover() | setProtectiveDrumCover(Boolean protectiveDrumCover) |
| `ProtectivePalletCover` | `Boolean` | Optional | Indicates that this is a protective pallet cover delivery. Defaults to 'not a protective pallet cover delivery' if not submitted.<br><br>**Default**: `false` | Boolean getProtectivePalletCover() | setProtectivePalletCover(Boolean protectivePalletCover) |
| `ReconsignmentFee` | `Boolean` | Optional | Indicates that this is a reconsignment fee delivery. Defaults to 'not a reconsignment fee delivery' if not submitted.<br><br>**Default**: `false` | Boolean getReconsignmentFee() | setReconsignmentFee(Boolean reconsignmentFee) |
| `RefrigeratedVan` | `Boolean` | Optional | Indicates that this is a refrigerated van delivery. Defaults to 'not a refrigerated van delivery' if not submitted.<br><br>**Default**: `false` | Boolean getRefrigeratedVan() | setRefrigeratedVan(Boolean refrigeratedVan) |
| `RegionalShipment` | `Boolean` | Optional | Indicates that this is a regional shipment delivery. Defaults to 'not a regional shipment delivery' if not submitted.<br><br>**Default**: `false` | Boolean getRegionalShipment() | setRegionalShipment(Boolean regionalShipment) |
| `RemoveDebris` | `Boolean` | Optional | Indicates that this is a removed debris delivery. Defaults to 'not a removed debris delivery' if not submitted.<br><br>**Default**: `false` | Boolean getRemoveDebris() | setRemoveDebris(Boolean removeDebris) |
| `SecurityInspection` | `Boolean` | Optional | Indicates that this is a security inspection delivery. Defaults to 'not a security inspection delivery' if not submitted.<br><br>**Default**: `false` | Boolean getSecurityInspection() | setSecurityInspection(Boolean securityInspection) |
| `SpecialEquipmentNeeded` | `Boolean` | Optional | Indicates that this is a special equipment needed delivery. Defaults to 'not a special equipment needed delivery' if not submitted.<br><br>**Default**: `false` | Boolean getSpecialEquipmentNeeded() | setSpecialEquipmentNeeded(Boolean specialEquipmentNeeded) |
| `Storage` | `Boolean` | Optional | Indicates that this is a storage delivery. Defaults to 'not a storage delivery' if not submitted.<br><br>**Default**: `false` | Boolean getStorage() | setStorage(Boolean storage) |
| `StopOff` | `Boolean` | Optional | Indicates that this is a stop off delivery. Defaults to 'not a stop off delivery' if not submitted.<br><br>**Default**: `false` | Boolean getStopOff() | setStopOff(Boolean stopOff) |
| `StraightTruck` | `Boolean` | Optional | Indicates that this is a straight truck delivery. Defaults to 'not a straight truck delivery' if not submitted.<br><br>**Default**: `false` | Boolean getStraightTruck() | setStraightTruck(Boolean straightTruck) |
| `TankerTruck` | `Boolean` | Optional | Indicates that this is a tanker truck delivery. Defaults to 'not a tanker truck delivery' if not submitted.<br><br>**Default**: `false` | Boolean getTankerTruck() | setTankerTruck(Boolean tankerTruck) |
| `TruckNotUsed` | `Boolean` | Optional | Indicates that this is a truck not used delivery. Defaults to 'not a truck not used delivery' if not submitted.<br><br>**Default**: `false` | Boolean getTruckNotUsed() | setTruckNotUsed(Boolean truckNotUsed) |
| `TeamCharge` | `Boolean` | Optional | Indicates that this is a team charge delivery. Defaults to 'not a team charge delivery' if not submitted.<br><br>**Default**: `false` | Boolean getTeamCharge() | setTeamCharge(Boolean teamCharge) |
| `TSACertification` | `Boolean` | Optional | Indicates that this is a TSA certification delivery. Defaults to 'not a TSA certification delivery' if not submitted.<br><br>**Default**: `false` | Boolean getTSACertification() | setTSACertification(Boolean tSACertification) |
| `DriverUnload` | `Boolean` | Optional | Indicates that this is a driver unload delivery. Defaults to 'not a driver unload delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDriverUnload() | setDriverUnload(Boolean driverUnload) |
| `DriverUnloadandCount` | `Boolean` | Optional | Indicates that this is a driver unload and count delivery. Defaults to 'not a driver unload and count delivery' if not submitted.<br><br>**Default**: `false` | Boolean getDriverUnloadandCount() | setDriverUnloadandCount(Boolean driverUnloadandCount) |
| `WeekendService` | `Boolean` | Optional | Indicates that this is a weekend service delivery. Defaults to 'not a weekend service delivery' if not submitted.<br><br>**Default**: `false` | Boolean getWeekendService() | setWeekendService(Boolean weekendService) |
| `WeightInspection` | `Boolean` | Optional | Indicates that this is a weight inspection delivery. Defaults to 'not a weight inspection delivery' if not submitted.<br><br>**Default**: `false` | Boolean getWeightInspection() | setWeightInspection(Boolean weightInspection) |
| `WeightVerification` | `Boolean` | Optional | Indicates that this is a weight verification delivery. Defaults to 'not a weight verification delivery' if not submitted.<br><br>**Default**: `false` | Boolean getWeightVerification() | setWeightVerification(Boolean weightVerification) |
| `ExtraLabor` | `Boolean` | Optional | Indicates that this is a extra labor delivery. Defaults to 'not a extra labor delivery' if not submitted.<br><br>**Default**: `false` | Boolean getExtraLabor() | setExtraLabor(Boolean extraLabor) |
| `AddressChangeNotification` | `Boolean` | Optional | Used in conjunction with DispositionMethod for Ancillary Service Endorsements on DHL Global Mail Domestic Label.  Defaults to false if not submitted.<br><br>**Default**: `false` | Boolean getAddressChangeNotification() | setAddressChangeNotification(Boolean addressChangeNotification) |
| `DispositionMethod` | [`DispositionMethodEnum`](../../doc/models/disposition-method-enum.md) | Optional | Used for ancillary endorsements.  Uses the carrier default if not submitted.<br><br>**Default**: `DispositionMethodEnum.ENUM_0` | DispositionMethodEnum getDispositionMethod() | setDispositionMethod(DispositionMethodEnum dispositionMethod) |
| `FreightHandlingType` | [`FreightHandlingTypeEnum`](../../doc/models/freight-handling-type-enum.md) | Optional | Used for setting outer handling unit type for freight shipments.<br><br>**Default**: `FreightHandlingTypeEnum.ENUM_0` | FreightHandlingTypeEnum getFreightHandlingType() | setFreightHandlingType(FreightHandlingTypeEnum freightHandlingType) |
| `FreightHandlingUnits` | `Integer` | Optional | The number of freight handling units in the shipment.<br><br>**Default**: `0` | Integer getFreightHandlingUnits() | setFreightHandlingUnits(Integer freightHandlingUnits) |
| `AlcoholShipment` | `Integer` | Optional | Used to inform carrier of type of alcohol shipment.  Defaults to none if not submitted.<br><br>**Default**: `0` | Integer getAlcoholShipment() | setAlcoholShipment(Integer alcoholShipment) |
| `ReturnLegPickup` | `Boolean` | Optional | Indicates if an item should be picked up from the recipient and returned to the shipper. Default to false if not submitted.<br><br>**Default**: `false` | Boolean getReturnLegPickup() | setReturnLegPickup(Boolean returnLegPickup) |
| `InboundShipment` | `Boolean` | Optional | Indicates if the shipment to be rated is an inbound shipment.<br><br>**Default**: `false` | Boolean getInboundShipment() | setInboundShipment(Boolean inboundShipment) |
| `BoLNumber` | `String` | Optional | Bill of Lading number associated with the shipment. | String getBoLNumber() | setBoLNumber(String boLNumber) |
| `ContentType` | [`ContentTypeEnum`](../../doc/models/content-type-enum.md) | Optional | Content type of materials in the shipment. | ContentTypeEnum getContentType() | setContentType(ContentTypeEnum contentType) |
| `MasterBoL` | `Boolean` | Optional | Indicates whether the shipment is the master shipment when using a master BOL.  Defaults to no regular shipment if not submitted or child shipment if not submitted and a MasterBoLnumber is passed.<br><br>**Default**: `false` | Boolean getMasterBoL() | setMasterBoL(Boolean masterBoL) |
| `MasterBoLNumber` | `String` | Optional | Master Bill of Lading number associated with the shipment. If the shipment is a child, this must be passed but MasterBoL omitted or set to false. | String getMasterBoLNumber() | setMasterBoLNumber(String masterBoLNumber) |
| `ShipToHold` | `Boolean` | Optional | Indicates whether the shipment should be held before shipping.  Defaults to not hold before shipping if omitted.<br><br>**Default**: `false` | Boolean getShipToHold() | setShipToHold(Boolean shipToHold) |
| `TemperatureService` | `Integer` | Optional | Indicates the type of temperature service selected for the shipment. Defaults to none if not submitted.<br><br>**Default**: `0` | Integer getTemperatureService() | setTemperatureService(Integer temperatureService) |
| `SmartPostIndiciaType` | `Integer` | Optional | Specify the indicia type associated with the smartpost shipment.<br><br>**Default**: `0` | Integer getSmartPostIndiciaType() | setSmartPostIndiciaType(Integer smartPostIndiciaType) |
| `SmartPostAncillaryEndorsement` | `Integer` | Optional | Indicates the SmartPost Ancillary Endorsement type selected for the shipment.<br><br>**Default**: `0` | Integer getSmartPostAncillaryEndorsement() | setSmartPostAncillaryEndorsement(Integer smartPostAncillaryEndorsement) |
| `SmartPostHubID` | `Integer` | Optional | Indicates the SmartPost Hub ID selected for the shipment. Mandatory for SmartPost.<br><br>**Default**: `0` | Integer getSmartPostHubID() | setSmartPostHubID(Integer smartPostHubID) |
| `SmartPostCustomerManifestID` | `String` | Optional | Customer designated manifest ID for SmartPost shipments. | String getSmartPostCustomerManifestID() | setSmartPostCustomerManifestID(String smartPostCustomerManifestID) |
| `SmartPostSecondaryBarcode` | `Integer` | Optional | Indicates the SmartPost Secondary Barcode Type selected for the shipment. | Integer getSmartPostSecondaryBarcode() | setSmartPostSecondaryBarcode(Integer smartPostSecondaryBarcode) |
| `LabelDetailMask` | [`LabelDetailMaskEnum`](../../doc/models/label-detail-mask-enum.md) | Optional | Indicates the label detail mask selected for the shipment. | LabelDetailMaskEnum getLabelDetailMask() | setLabelDetailMask(LabelDetailMaskEnum labelDetailMask) |
| `RMA` | `String` | Optional | Used to associate an Return merchandise authorization with a returns shipment. | String getRMA() | setRMA(String rMA) |
| `ColdChain` | `Boolean` | Optional | Indicates whether the shipment requires a cold chain service. This is for shipment freight level. Note cold chain is available for parcel at package level.<br><br>**Default**: `false` | Boolean getColdChain() | setColdChain(Boolean coldChain) |
| `HolidayDelivery` | `Boolean` | Optional | Indicates whether the shipment requires a holiday delivery service.<br><br>**Default**: `false` | Boolean getHolidayDelivery() | setHolidayDelivery(Boolean holidayDelivery) |
| `HolidayPickup` | `Boolean` | Optional | Indicates whether the shipment requires a holiday pickup.<br><br>**Default**: `false` | Boolean getHolidayPickup() | setHolidayPickup(Boolean holidayPickup) |
| `SundayDelivery` | `Boolean` | Optional | Indicates whether the shipment requires a sunday delivery service.<br><br>**Default**: `false` | Boolean getSundayDelivery() | setSundayDelivery(Boolean sundayDelivery) |
| `WeekendDelivery` | `Boolean` | Optional | Indicates whether the shipment requires a weekend delivery service.<br><br>**Default**: `false` | Boolean getWeekendDelivery() | setWeekendDelivery(Boolean weekendDelivery) |
| `WeekendPickup` | `Boolean` | Optional | Indicates whether the shipment requires a weekend pickup.<br><br>**Default**: `false` | Boolean getWeekendPickup() | setWeekendPickup(Boolean weekendPickup) |
| `ExcessDeclaredValue` | `Double` | Optional | Excess Declared Value amount.<br><br>**Default**: `0d` | Double getExcessDeclaredValue() | setExcessDeclaredValue(Double excessDeclaredValue) |
| `ShowPostageOnLabel` | `Boolean` | Optional | Indicates whether the label will contain the postage value.<br><br>**Default**: `false` | Boolean getShowPostageOnLabel() | setShowPostageOnLabel(Boolean showPostageOnLabel) |
| `PouchID` | `Integer` | Optional | Pouch that this shipment is part of.<br><br>**Default**: `0` | Integer getPouchID() | setPouchID(Integer pouchID) |
| `ITARLicenseExemptionNumber` | `String` | Optional | International Trade in Arms Regulations License or Exemption Number of the company sending the shipment. | String getITARLicenseExemptionNumber() | setITARLicenseExemptionNumber(String iTARLicenseExemptionNumber) |
| `ITARPreDepartureITN` | `String` | Optional | The Internal Transaction Number returned by the Census Bureau. | String getITARPreDepartureITN() | setITARPreDepartureITN(String iTARPreDepartureITN) |
| `FirstDelivery` | `Boolean` | Optional | Indicates whether the shipment requires the First Delivery special service.<br><br>**Default**: `false` | Boolean getFirstDelivery() | setFirstDelivery(Boolean firstDelivery) |
| `FreeDomicile` | `Boolean` | Optional | Indicates whether the shipment requires the Free Domicile special service.<br><br>**Default**: `false` | Boolean getFreeDomicile() | setFreeDomicile(Boolean freeDomicile) |
| `NoonDelivery` | `Boolean` | Optional | Indicates whether the shipment requires the Noon Delivery special service.<br><br>**Default**: `false` | Boolean getNoonDelivery() | setNoonDelivery(Boolean noonDelivery) |
| `CollectAmount` | `Double` | Optional | The amount to be collected from consignee.<br><br>**Default**: `0d` | Double getCollectAmount() | setCollectAmount(Double collectAmount) |
| `HazardousOtherRequiredInformation` | `String` | Optional | Other Hazardous Required Information for the shipment. | String getHazardousOtherRequiredInformation() | setHazardousOtherRequiredInformation(String hazardousOtherRequiredInformation) |
| `HazardousInstructions` | `String` | Optional | Hazardous Instructions for the shipment. | String getHazardousInstructions() | setHazardousInstructions(String hazardousInstructions) |
| `HazardousAdditionalHandling` | `String` | Optional | Additional handling measures for hazardous package. | String getHazardousAdditionalHandling() | setHazardousAdditionalHandling(String hazardousAdditionalHandling) |
| `CashAdditionalAmount` | `Double` | Optional | Additional cash that can be required for miscellaneous reasons.<br><br>**Default**: `0d` | Double getCashAdditionalAmount() | setCashAdditionalAmount(Double cashAdditionalAmount) |
| `CashAdditionalDescription` | `String` | Optional | Description of why additional cash is required. | String getCashAdditionalDescription() | setCashAdditionalDescription(String cashAdditionalDescription) |
| `ImportDelivery` | `Boolean` | Optional | Used to indicate whether the shipment will processed using import control | Boolean getImportDelivery() | setImportDelivery(Boolean importDelivery) |
| `ImportDeliveryLabelType` | `Integer` | Optional | Type of label to be generated for an import delivery.<br><br>**Default**: `0` | Integer getImportDeliveryLabelType() | setImportDeliveryLabelType(Integer importDeliveryLabelType) |
| `CommercialInvoiceRemoval` | `Boolean` | Optional | Used to indicate to the carrier to remove the Commercial Invoice from the user's shipment before the shipment is delivered | Boolean getCommercialInvoiceRemoval() | setCommercialInvoiceRemoval(Boolean commercialInvoiceRemoval) |
| `HoldForPickup` | `Boolean` | Optional | Used to indicate whether the shipment should be held for pickup | Boolean getHoldForPickup() | setHoldForPickup(Boolean holdForPickup) |
| `NYCMetro` | `Boolean` | Optional | Use to indicate if delivery location is within New York City metro area | Boolean getNYCMetro() | setNYCMetro(Boolean nYCMetro) |
| `TwoHourSpecialDelivery` | `Boolean` | Optional | Indicates whether the shipment requires a two hour special delivery service. | Boolean getTwoHourSpecialDelivery() | setTwoHourSpecialDelivery(Boolean twoHourSpecialDelivery) |
| `BlanketService` | `Boolean` | Optional | Indicates whether the shipment requires a blanket service. | Boolean getBlanketService() | setBlanketService(Boolean blanketService) |
| `Stackable` | `Boolean` | Optional | Indicates whether the shipment is stackable. | Boolean getStackable() | setStackable(Boolean stackable) |
| `Turnkey` | `Boolean` | Optional | Indicates whether the shipment is turnkey. | Boolean getTurnkey() | setTurnkey(Boolean turnkey) |
| `BlanketServiceChilled` | `Boolean` | Optional | Indicates whether the shipment requires a chilled blanket service. | Boolean getBlanketServiceChilled() | setBlanketServiceChilled(Boolean blanketServiceChilled) |
| `BlanketServiceFrozen` | `Boolean` | Optional | Indicates whether the shipment requires a frozen blanket service. | Boolean getBlanketServiceFrozen() | setBlanketServiceFrozen(Boolean blanketServiceFrozen) |
| `ProactiveResponse` | `Boolean` | Optional | Service that monitors a shipment for delays and will attempt to reroute is there are delays avoiding failure in service. Typically used for temperature sensitive or life-saving shipments. | Boolean getProactiveResponse() | setProactiveResponse(Boolean proactiveResponse) |
| `LimitedAccessPickupType` | `Integer` | Optional | Numeric identifer for the type of limited access pickup.  Defaults to no limited access delivery if not submitted.<br><br>**Default**: `0` | Integer getLimitedAccessPickupType() | setLimitedAccessPickupType(Integer limitedAccessPickupType) |
| `LimitedAccessDeliveryType` | `Integer` | Optional | Numeric identifer for the type of limited access delivery.  Defaults to no limited access delivery if not submitted.<br><br>**Default**: `0` | Integer getLimitedAccessDeliveryType() | setLimitedAccessDeliveryType(Integer limitedAccessDeliveryType) |
| `DiagnosticSpecimens` | `Boolean` | Optional | Used to indicate whether the shipment contains Biological substances | Boolean getDiagnosticSpecimens() | setDiagnosticSpecimens(Boolean diagnosticSpecimens) |
| `AlcoholicBeverages` | `Boolean` | Optional | Used to indicate whether the shipment contains alcoholic beverages | Boolean getAlcoholicBeverages() | setAlcoholicBeverages(Boolean alcoholicBeverages) |
| `Perishables` | `Boolean` | Optional | Used to indicate whether the shipment contains perishables | Boolean getPerishables() | setPerishables(Boolean perishables) |
| `Plants` | `Boolean` | Optional | Used to indicate whether the shipment contains plants | Boolean getPlants() | setPlants(Boolean plants) |
| `Seeds` | `Boolean` | Optional | Used to indicate whether the shipment contains seeds | Boolean getSeeds() | setSeeds(Boolean seeds) |
| `SpecialExceptions` | `Boolean` | Optional | Used to indicate whether the shipment contains special exceptions | Boolean getSpecialExceptions() | setSpecialExceptions(Boolean specialExceptions) |
| `Tobacco` | `Boolean` | Optional | Used to indicate whether the shipment contains tobacco | Boolean getTobacco() | setTobacco(Boolean tobacco) |
| `DropAtCarrierFacility` | `Boolean` | Optional | Used to indicate whether the shipment will be dropped at a carrier facility | Boolean getDropAtCarrierFacility() | setDropAtCarrierFacility(Boolean dropAtCarrierFacility) |
| `PickupNotification` | `Boolean` | Optional | Indicates whether the shipment requires a Pickup Notification. | Boolean getPickupNotification() | setPickupNotification(Boolean pickupNotification) |
| `CFSDelivery` | `Boolean` | Optional | Indicates whether the shipment requires container freight station delivery. | Boolean getCFSDelivery() | setCFSDelivery(Boolean cFSDelivery) |
| `CFSPickup` | `Boolean` | Optional | Indicates whether the shipment requires container freight station pickup. | Boolean getCFSPickup() | setCFSPickup(Boolean cFSPickup) |
| `LabelRequired` | `Boolean` | Optional | Indicates if a label needs to be delivered by the driver at time of pickup.  Defaults to not required if not submitted.<br><br>**Default**: `false` | Boolean getLabelRequired() | setLabelRequired(Boolean labelRequired) |
| `PrintAsYouGo` | [`PrintAsYouGo`](../../doc/models/print-as-you-go.md) | Optional | Container element the Print As You Go option. | PrintAsYouGo getPrintAsYouGo() | setPrintAsYouGo(PrintAsYouGo printAsYouGo) |
| `VariableHandlingCharge` | [`VariableHandlingCharge`](../../doc/models/variable-handling-charge.md) | Optional | Container for variable handling charge elements. | VariableHandlingCharge getVariableHandlingCharge() | setVariableHandlingCharge(VariableHandlingCharge variableHandlingCharge) |
| `ExternalSystemType` | `Integer` | Optional | External system type (e.g. CargoWiseOne eHub) to send message for.<br><br>**Default**: `0` | Integer getExternalSystemType() | setExternalSystemType(Integer externalSystemType) |
| `IsMasterCarton` | `Boolean` | Optional | Indicates whether shipment is master carton (currently used for UPS ww economy only)<br><br>**Default**: `false` | Boolean getIsMasterCarton() | setIsMasterCarton(Boolean isMasterCarton) |
| `Sender` | [`Sender2`](../../doc/models/sender-2.md) | Optional | Container to allow the customization of the sender address details associated with the transaction. | Sender2 getSender() | setSender(Sender2 sender) |
| `Receiver` | [`Receiver4`](../../doc/models/receiver-4.md) | Required | Container for the receiver address details associated with the transaction. | Receiver4 getReceiver() | setReceiver(Receiver4 receiver) |
| `ReceiverIdentity` | [`ReceiverIdentity`](../../doc/models/receiver-identity.md) | Optional | Container element for receiver identification details. | ReceiverIdentity getReceiverIdentity() | setReceiverIdentity(ReceiverIdentity receiverIdentity) |
| `ReturnTo` | [`ReturnTo2`](../../doc/models/return-to-2.md) | Optional | Container for any return address assocaited with the transaction. | ReturnTo2 getReturnTo() | setReturnTo(ReturnTo2 returnTo) |
| `CODRemittanceAddress` | [`CODRemittanceAddress1`](../../doc/models/cod-remittance-address-1.md) | Optional | Container for the COD remittance address details. | CODRemittanceAddress1 getCODRemittanceAddress() | setCODRemittanceAddress(CODRemittanceAddress1 cODRemittanceAddress) |
| `Billing` | [`Billing4`](../../doc/models/billing-4.md) | Optional | Container for billing details associated with the transaction. | Billing4 getBilling() | setBilling(Billing4 billing) |
| `LabelOriginAddress` | [`LabelOriginAddress`](../../doc/models/label-origin-address.md) | Optional | Container to allow the customization of the sender address details associated with the label | LabelOriginAddress getLabelOriginAddress() | setLabelOriginAddress(LabelOriginAddress labelOriginAddress) |
| `HomeDelivery` | [`HomeDelivery`](../../doc/models/home-delivery.md) | Optional | Container for home delivery details. | HomeDelivery getHomeDelivery() | setHomeDelivery(HomeDelivery homeDelivery) |
| `Invoice` | [`Invoice`](../../doc/models/invoice.md) | Optional | Container for address details where the shipment costs should be invoiced. | Invoice getInvoice() | setInvoice(Invoice invoice) |
| `Assured` | [`Assured`](../../doc/models/assured.md) | Optional | Container for the address of the individual to be assured. | Assured getAssured() | setAssured(Assured assured) |
| `Notifications` | [`Notifications1`](../../doc/models/notifications-1.md) | Optional | Container for email notifications. | Notifications1 getNotifications() | setNotifications(Notifications1 notifications) |
| `International` | [`International8`](../../doc/models/international-8.md) | Optional | Container for international details associated with the shipment. | International8 getInternational() | setInternational(International8 international) |
| `Rates` | [`Rates4`](../../doc/models/rates-4.md) | Optional | Container all rates associated with the transaction. | Rates4 getRates() | setRates(Rates4 rates) |
| `Packages` | [`Packages6`](../../doc/models/packages-6.md) | Optional | Container for all packages associated with the transaction. | Packages6 getPackages() | setPackages(Packages6 packages) |
| `Freight` | [`Freight2`](../../doc/models/freight-2.md) | Optional | Container for freight specific values | Freight2 getFreight() | setFreight(Freight2 freight) |
| `UseConfiguredLetterHeadImage` | `Boolean` | Optional | Parameter used to override the configured value for the letter head image. Defaults to the configured value held within shipment server. | Boolean getUseConfiguredLetterHeadImage() | setUseConfiguredLetterHeadImage(Boolean useConfiguredLetterHeadImage) |
| `UseConfiguredSignatureImage` | `Boolean` | Optional | Parameter used to override the configured value for the signature image. Defaults to the configured value held within shipment server. | Boolean getUseConfiguredSignatureImage() | setUseConfiguredSignatureImage(Boolean useConfiguredSignatureImage) |
| `AutomatePostageMeterAdd` | `Boolean` | Optional | Indicates automatic handling of postage meter add transaction on a ship.<br><br>**Default**: `false` | Boolean getAutomatePostageMeterAdd() | setAutomatePostageMeterAdd(Boolean automatePostageMeterAdd) |
| `AutomatePostageMeterRate` | `Double` | Optional | Indicates amount to debit a meter during automatic handling of postage meter add transaction.<br><br>**Default**: `0d` | Double getAutomatePostageMeterRate() | setAutomatePostageMeterRate(Double automatePostageMeterRate) |
| `AutomatePostageMeterSerialNumber` | `String` | Optional | Meter Serial number used for automating postage add transactions. | String getAutomatePostageMeterSerialNumber() | setAutomatePostageMeterSerialNumber(String automatePostageMeterSerialNumber) |
| `MeterModeShipment` | `Boolean` | Optional | Set to true when in Parcel Mode and meter needs to be tripped or when in Postage Mode and label needs to be requested.<br><br>**Default**: `false` | Boolean getMeterModeShipment() | setMeterModeShipment(Boolean meterModeShipment) |
| `HazardousHelpLine` | [`HazardousHelpLine`](../../doc/models/hazardous-help-line.md) | Optional | Container for the Hazardous Helpline details associated with the transaction. | HazardousHelpLine getHazardousHelpLine() | setHazardousHelpLine(HazardousHelpLine hazardousHelpLine) |
| `HazardousHelpLineInfectious` | [`HazardousHelpLineInfectious`](../../doc/models/hazardous-help-line-infectious.md) | Optional | Container for the Infectious Helpline details associated with the transaction. | HazardousHelpLineInfectious getHazardousHelpLineInfectious() | setHazardousHelpLineInfectious(HazardousHelpLineInfectious hazardousHelpLineInfectious) |
| `DropOffType` | [`DropOffTypeEnum`](../../doc/models/drop-off-type-enum.md) | Optional | Type of drop off for the shipment. | DropOffTypeEnum getDropOffType() | setDropOffType(DropOffTypeEnum dropOffType) |
| `UseCartonization` | `Boolean` | Optional | Indicates whether to use return cartonized packages.<br><br>**Default**: `false` | Boolean getUseCartonization() | setUseCartonization(Boolean useCartonization) |
| `Cartonization` | [`Cartonization2`](../../doc/models/cartonization-2.md) | Optional | Container for cartonization data for this transaction. | Cartonization2 getCartonization() | setCartonization(Cartonization2 cartonization) |
| `CommercialInvoice` | [`CommercialInvoice`](../../doc/models/commercial-invoice.md) | Optional | Container to allow the customization of the commercial invoice details associated with the transaction. | CommercialInvoice getCommercialInvoice() | setCommercialInvoice(CommercialInvoice commercialInvoice) |
| `Rush` | `Boolean` | Optional | Indicates whether shipment is to be rushed.<br><br>**Default**: `false` | Boolean getRush() | setRush(Boolean rush) |
| `CustomsOptions` | [`CustomsOptions`](../../doc/models/customs-options.md) | Optional | Identifies the customs options for the consolidated shipment. | CustomsOptions getCustomsOptions() | setCustomsOptions(CustomsOptions customsOptions) |
| `ShipAfterRateResult` | [`ShipAfterRateResultEnum`](../../doc/models/ship-after-rate-result-enum.md) | Optional | For certain carriers where a rate request is performed prior to shipping this node enables shippers a level of control on when a ship will be attempted after the rate result. Default behaviour is for shipping to occur on success only, options for partial success and failure (All) are also available.<br><br>**Default**: `ShipAfterRateResultEnum.SUCCESSONLY` | ShipAfterRateResultEnum getShipAfterRateResult() | setShipAfterRateResult(ShipAfterRateResultEnum shipAfterRateResult) |
| `PersonalShipping` | [`PersonalShipping1`](../../doc/models/personal-shipping-1.md) | Optional | Container for personal shipping elements. | PersonalShipping1 getPersonalShipping() | setPersonalShipping(PersonalShipping1 personalShipping) |
| `ServiceTypeExternalSystemCode` | `String` | Optional | Carrier and service level code for external systems translation. | String getServiceTypeExternalSystemCode() | setServiceTypeExternalSystemCode(String serviceTypeExternalSystemCode) |
| `Diagnostics` | [`Diagnostics`](../../doc/models/diagnostics.md) | Optional | Container for logging and diagnostic override elements. | Diagnostics getDiagnostics() | setDiagnostics(Diagnostics diagnostics) |
| `Identification` | [`Identification`](../../doc/models/identification.md) | Optional | Container for client identification elements. | Identification getIdentification() | setIdentification(Identification identification) |
| `SourceApplication` | [`SourceApplication`](../../doc/models/source-application.md) | Optional | Container for app specific source identification elements. | SourceApplication getSourceApplication() | setSourceApplication(SourceApplication sourceApplication) |

## Example (as XML)

```xml
<wtg:PierbridgeShipRequest xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:UpdateShipmentType xmlns:wtg="https://www.wisetechglobal.com/">None</wtg:UpdateShipmentType>
  <wtg:UpdateShipmentID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:UpdateShipmentID>
  <wtg:DisplayRateTypeID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:DisplayRateTypeID>
  <wtg:UpdateRateTypeID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:UpdateRateTypeID>
  <wtg:OtherRateTypeID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:OtherRateTypeID>
  <wtg:IsReturn xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:IsReturn>
  <wtg:DisableValidation xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DisableValidation>
  <wtg:DisableExecution xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DisableExecution>
  <wtg:ExportInvoiceData xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ExportInvoiceData>
  <wtg:ResetWayBillNumbers xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ResetWayBillNumbers>
  <wtg:ReverseSenderReceiverAddress xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReverseSenderReceiverAddress>
  <wtg:UserName xmlns:wtg="https://www.wisetechglobal.com/"></wtg:UserName>
  <wtg:ISOCurrencyId xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ISOCurrencyId>
  <wtg:DocketConsolidation xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DocketConsolidation>
  <wtg:IsWorldEase xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:IsWorldEase>
  <wtg:CommercialInvoicePaperless xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CommercialInvoicePaperless>
  <wtg:CertificateOfOriginPaperless xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CertificateOfOriginPaperless>
  <wtg:CommercialInvoiceWithheld xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CommercialInvoiceWithheld>
  <wtg:AdditionalHardcopyDocumentation xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AdditionalHardcopyDocumentation>
  <wtg:RateGroup xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:RateGroup>
  <wtg:FilterMode xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:FilterMode>
  <wtg:SortMode xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:SortMode>
  <wtg:InsuranceProvider xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:InsuranceProvider>
  <wtg:Live xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Live>
  <wtg:NumberOfPieces xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:NumberOfPieces>
  <wtg:PharmacyDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PharmacyDelivery>
  <wtg:CostCenterID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:CostCenterID>
  <wtg:CostCenterBarcodeIndicator xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CostCenterBarcodeIndicator>
  <wtg:PackageIDBarcodeIndicator xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PackageIDBarcodeIndicator>
  <wtg:ShipForUserID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ShipForUserID>
  <wtg:Carrier xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Carrier>
  <wtg:ServiceType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ServiceType>
  <wtg:PackageType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageType>
  <wtg:SuggestedServiceType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:SuggestedServiceType>
  <wtg:CustomerServiceType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:CustomerServiceType>
  <wtg:CustomerCostOption xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:CustomerCostOption>
  <wtg:SaturdayDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SaturdayDelivery>
  <wtg:SaturdayPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SaturdayPickup>
  <wtg:SundayPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SundayPickup>
  <wtg:AfterHoursDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AfterHoursDelivery>
  <wtg:CorrectedBOLFee xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CorrectedBOLFee>
  <wtg:ResidentialFurnitureDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ResidentialFurnitureDelivery>
  <wtg:TarpingSurcharge xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:TarpingSurcharge>
  <wtg:DeliverOnlyToShipAddress xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DeliverOnlyToShipAddress>
  <wtg:DeliverOnlyToAddressee xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DeliverOnlyToAddressee>
  <wtg:DryIceForMedicalUse xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DryIceForMedicalUse>
  <wtg:CarbonNeutral xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CarbonNeutral>
  <wtg:ShipmentRequisitionID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ShipmentRequisitionID>
  <wtg:PendingID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PendingID>
  <wtg:TotalCharge xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TotalCharge>
  <wtg:CustomerID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:CustomerID>
  <wtg:AccountID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:AccountID>
  <wtg:ShippingKeyID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ShippingKeyID>
  <wtg:RouteID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:RouteID>
  <wtg:RouteCode xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:RouteCode>
  <wtg:RequiresASN xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:RequiresASN>
  <wtg:Security xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Security>
  <wtg:PriorDeliveryNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PriorDeliveryNotification>
  <wtg:Unpack xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Unpack>
  <wtg:HealthInsurance xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HealthInsurance>
  <wtg:SpecialDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SpecialDelivery>
  <wtg:ForkliftDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ForkliftDelivery>
  <wtg:InsidePickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:InsidePickup>
  <wtg:InsideDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:InsideDelivery>
  <wtg:DoNotBreakDown xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DoNotBreakDown>
  <wtg:DoNotStackPallets xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DoNotStackPallets>
  <wtg:Oversized xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Oversized>
  <wtg:TopLoadOnly xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:TopLoadOnly>
  <wtg:Food xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Food>
  <wtg:Poison xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Poison>
  <wtg:ConsolidatedShipmentID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ConsolidatedShipmentID>
  <wtg:ConsolidatedShipmentTypeID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ConsolidatedShipmentTypeID>
  <wtg:QuickRate xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:QuickRate>
  <wtg:Truckload xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Truckload>
  <wtg:FreightAllKinds xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:FreightAllKinds>
  <wtg:Interline xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Interline>
  <wtg:LoadingDockDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LoadingDockDelivery>
  <wtg:ConstructionSitePickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ConstructionSitePickup>
  <wtg:ConstructionSiteDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ConstructionSiteDelivery>
  <wtg:TradeShowPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:TradeShowPickup>
  <wtg:TradeShowDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:TradeShowDelivery>
  <wtg:LiftGateDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LiftGateDelivery>
  <wtg:LiftGatePickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LiftGatePickup>
  <wtg:AppointmentDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AppointmentDelivery>
  <wtg:AppointmentPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AppointmentPickup>
  <wtg:NineAMDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NineAMDelivery>
  <wtg:DeliveryWindow xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DeliveryWindow>
  <wtg:DeliverToDoor xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DeliverToDoor>
  <wtg:UnloadFreightAtDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:UnloadFreightAtDelivery>
  <wtg:LoadFreightAtPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LoadFreightAtPickup>
  <wtg:WhiteGlove xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:WhiteGlove>
  <wtg:TwoManDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:TwoManDelivery>
  <wtg:PalletExchange xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PalletExchange>
  <wtg:SortAndSegregate xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SortAndSegregate>
  <wtg:Wholesaler xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Wholesaler>
  <wtg:TobaccoReportingCharge xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:TobaccoReportingCharge>
  <wtg:Bulkhead xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Bulkhead>
  <wtg:CallBeforeDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CallBeforeDelivery>
  <wtg:HighCostDeliverySurcharge xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HighCostDeliverySurcharge>
  <wtg:LimitedAccessDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LimitedAccessDelivery>
  <wtg:RemoteLocationSurcharge xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:RemoteLocationSurcharge>
  <wtg:AMDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AMDelivery>
  <wtg:SingleShipment xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SingleShipment>
  <wtg:LimitedAccessPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LimitedAccessPickup>
  <wtg:AirportPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AirportPickup>
  <wtg:CampPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CampPickup>
  <wtg:CertifiedPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CertifiedPickup>
  <wtg:ChurchPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ChurchPickup>
  <wtg:CountryClubPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CountryClubPickup>
  <wtg:CommercialPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CommercialPickup>
  <wtg:DockPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DockPickup>
  <wtg:DeclaredValuePickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DeclaredValuePickup>
  <wtg:SchoolPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SchoolPickup>
  <wtg:FarmPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:FarmPickup>
  <wtg:FlatbedPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:FlatbedPickup>
  <wtg:GovernmentSitePickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:GovernmentSitePickup>
  <wtg:GroceryWarehousePickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:GroceryWarehousePickup>
  <wtg:HospitalPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HospitalPickup>
  <wtg:HotelPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HotelPickup>
  <wtg:MallPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:MallPickup>
  <wtg:MilitaryInstallationPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:MilitaryInstallationPickup>
  <wtg:MineSitePickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:MineSitePickup>
  <wtg:NativeAmericanReservationPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NativeAmericanReservationPickup>
  <wtg:NonBusinessHoursPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NonBusinessHoursPickup>
  <wtg:NonCommercialPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NonCommercialPickup>
  <wtg:NursingHomePickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NursingHomePickup>
  <wtg:OversizedPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OversizedPickup>
  <wtg:FairAmusementParkPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:FairAmusementParkPickup>
  <wtg:PierPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PierPickup>
  <wtg:PalletJackPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PalletJackPickup>
  <wtg:PrisonPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PrisonPickup>
  <wtg:ResortPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ResortPickup>
  <wtg:SortSegregatePickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SortSegregatePickup>
  <wtg:SelfStoragePickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SelfStoragePickup>
  <wtg:UtilitySitePickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:UtilitySitePickup>
  <wtg:PalletExchangePickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PalletExchangePickup>
  <wtg:DockTransferPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DockTransferPickup>
  <wtg:AirportDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AirportDelivery>
  <wtg:AdvancedCollection xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AdvancedCollection>
  <wtg:CampDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CampDelivery>
  <wtg:ChurchDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ChurchDelivery>
  <wtg:CountryClubDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CountryClubDelivery>
  <wtg:CommercialDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CommercialDelivery>
  <wtg:DistributionCenterDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DistributionCenterDelivery>
  <wtg:DeclaredValueDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DeclaredValueDelivery>
  <wtg:SchoolDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SchoolDelivery>
  <wtg:EmergencyDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:EmergencyDelivery>
  <wtg:FarmDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:FarmDelivery>
  <wtg:FlatbedDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:FlatbedDelivery>
  <wtg:GovernmentSiteDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:GovernmentSiteDelivery>
  <wtg:GroceryWarehouseDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:GroceryWarehouseDelivery>
  <wtg:HospitalDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HospitalDelivery>
  <wtg:HotelDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HotelDelivery>
  <wtg:MallDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:MallDelivery>
  <wtg:MilitaryInstallationDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:MilitaryInstallationDelivery>
  <wtg:MineSiteDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:MineSiteDelivery>
  <wtg:NativeAmericanReservationDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NativeAmericanReservationDelivery>
  <wtg:NonBusinessHoursDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NonBusinessHoursDelivery>
  <wtg:NonCommercialDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NonCommercialDelivery>
  <wtg:NursingHomeDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NursingHomeDelivery>
  <wtg:OversizedDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OversizedDelivery>
  <wtg:FairAmusementParkDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:FairAmusementParkDelivery>
  <wtg:PierDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PierDelivery>
  <wtg:PalletJackDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PalletJackDelivery>
  <wtg:PrisonDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PrisonDelivery>
  <wtg:ResortDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ResortDelivery>
  <wtg:SortSegregateDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SortSegregateDelivery>
  <wtg:SelfStorageDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SelfStorageDelivery>
  <wtg:UtilitySiteDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:UtilitySiteDelivery>
  <wtg:PalletExchangeDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PalletExchangeDelivery>
  <wtg:DockTransferDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DockTransferDelivery>
  <wtg:AfterHoursCharge xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AfterHoursCharge>
  <wtg:AirFreight xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AirFreight>
  <wtg:AirBag xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AirBag>
  <wtg:ArbitraryCharge xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ArbitraryCharge>
  <wtg:BagLiner xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:BagLiner>
  <wtg:BlindShipment xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:BlindShipment>
  <wtg:Bobtail xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Bobtail>
  <wtg:InBondShipment xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:InBondShipment>
  <wtg:BeyondIndirectService xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:BeyondIndirectService>
  <wtg:NorthboundCanadianBorderCrossingDocumentHandlingFee xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NorthboundCanadianBorderCrossingDocumentHandlingFee>
  <wtg:CapacityLoadPup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CapacityLoadPup>
  <wtg:CapacityLoadTrailer xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CapacityLoadTrailer>
  <wtg:ChassisTruck xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ChassisTruck>
  <wtg:ChangeofBOL xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ChangeofBOL>
  <wtg:Consolidation xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Consolidation>
  <wtg:CorrectedBOL xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CorrectedBOL>
  <wtg:CranePermits xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CranePermits>
  <wtg:RedelivertoConsignee xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:RedelivertoConsignee>
  <wtg:CrossDock xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:CrossDock>
  <wtg:DescriptionInspection xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DescriptionInspection>
  <wtg:Detention xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Detention>
  <wtg:DelayCharge xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DelayCharge>
  <wtg:DriverAssistance xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DriverAssistance>
  <wtg:Drayage xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Drayage>
  <wtg:DropPull xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DropPull>
  <wtg:DryRun xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DryRun>
  <wtg:Excessivevalue xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Excessivevalue>
  <wtg:ExportShipment xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ExportShipment>
  <wtg:FlatTrack xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:FlatTrack>
  <wtg:ShipmentContainsFood xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ShipmentContainsFood>
  <wtg:Forklift xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Forklift>
  <wtg:HawaiianWillCall xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HawaiianWillCall>
  <wtg:HighDockEquipmentNeeded xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HighDockEquipmentNeeded>
  <wtg:HomeLandSecurity xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HomeLandSecurity>
  <wtg:HolidayWeekendService xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HolidayWeekendService>
  <wtg:ImportShipment xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ImportShipment>
  <wtg:InboundFreight xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:InboundFreight>
  <wtg:InterlineShipment xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:InterlineShipment>
  <wtg:InterRegionalShipment xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:InterRegionalShipment>
  <wtg:HandlingandLabeling xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HandlingandLabeling>
  <wtg:LiquorPermit xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LiquorPermit>
  <wtg:DriverLoad xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DriverLoad>
  <wtg:DriverLoadandCount xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DriverLoadandCount>
  <wtg:DriverLoadUnload xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DriverLoadUnload>
  <wtg:LumperService xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LumperService>
  <wtg:Layover xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Layover>
  <wtg:MarkingorTagging xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:MarkingorTagging>
  <wtg:NotifyBeforeDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NotifyBeforeDelivery>
  <wtg:Over750Under6 xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Over750Under6>
  <wtg:OilSands xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OilSands>
  <wtg:OpenTopTruck xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OpenTopTruck>
  <wtg:OverDimensionFreight xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:OverDimensionFreight>
  <wtg:Overweight xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Overweight>
  <wtg:Pallet xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Pallet>
  <wtg:ProtectFromHeat xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ProtectFromHeat>
  <wtg:ProtectFromFreezing xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ProtectFromFreezing>
  <wtg:ProtectFromFreezingCanada xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ProtectFromFreezingCanada>
  <wtg:Permit xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Permit>
  <wtg:ProtectiveService xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ProtectiveService>
  <wtg:ProtectiveDrumCover xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ProtectiveDrumCover>
  <wtg:ProtectivePalletCover xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ProtectivePalletCover>
  <wtg:ReconsignmentFee xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReconsignmentFee>
  <wtg:RefrigeratedVan xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:RefrigeratedVan>
  <wtg:RegionalShipment xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:RegionalShipment>
  <wtg:RemoveDebris xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:RemoveDebris>
  <wtg:SecurityInspection xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SecurityInspection>
  <wtg:SpecialEquipmentNeeded xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SpecialEquipmentNeeded>
  <wtg:Storage xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Storage>
  <wtg:StopOff xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:StopOff>
  <wtg:StraightTruck xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:StraightTruck>
  <wtg:TankerTruck xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:TankerTruck>
  <wtg:TruckNotUsed xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:TruckNotUsed>
  <wtg:TeamCharge xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:TeamCharge>
  <wtg:TSACertification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:TSACertification>
  <wtg:DriverUnload xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DriverUnload>
  <wtg:DriverUnloadandCount xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DriverUnloadandCount>
  <wtg:WeekendService xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:WeekendService>
  <wtg:WeightInspection xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:WeightInspection>
  <wtg:WeightVerification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:WeightVerification>
  <wtg:ExtraLabor xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ExtraLabor>
  <wtg:AddressChangeNotification xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AddressChangeNotification>
  <wtg:DispositionMethod xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:DispositionMethod>
  <wtg:FreightHandlingType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:FreightHandlingType>
  <wtg:FreightHandlingUnits xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:FreightHandlingUnits>
  <wtg:AlcoholShipment xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:AlcoholShipment>
  <wtg:ReturnLegPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ReturnLegPickup>
  <wtg:InboundShipment xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:InboundShipment>
  <wtg:MasterBoL xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:MasterBoL>
  <wtg:ShipToHold xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ShipToHold>
  <wtg:TemperatureService xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TemperatureService>
  <wtg:SmartPostIndiciaType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:SmartPostIndiciaType>
  <wtg:SmartPostAncillaryEndorsement xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:SmartPostAncillaryEndorsement>
  <wtg:SmartPostHubID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:SmartPostHubID>
  <wtg:ColdChain xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ColdChain>
  <wtg:HolidayDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HolidayDelivery>
  <wtg:HolidayPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:HolidayPickup>
  <wtg:SundayDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:SundayDelivery>
  <wtg:WeekendDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:WeekendDelivery>
  <wtg:WeekendPickup xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:WeekendPickup>
  <wtg:ExcessDeclaredValue xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ExcessDeclaredValue>
  <wtg:ShowPostageOnLabel xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:ShowPostageOnLabel>
  <wtg:PouchID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PouchID>
  <wtg:FirstDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:FirstDelivery>
  <wtg:FreeDomicile xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:FreeDomicile>
  <wtg:NoonDelivery xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NoonDelivery>
  <wtg:CollectAmount xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:CollectAmount>
  <wtg:CashAdditionalAmount xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:CashAdditionalAmount>
  <wtg:ImportDeliveryLabelType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ImportDeliveryLabelType>
  <wtg:LimitedAccessPickupType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:LimitedAccessPickupType>
  <wtg:LimitedAccessDeliveryType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:LimitedAccessDeliveryType>
  <wtg:LabelRequired xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:LabelRequired>
  <wtg:ExternalSystemType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ExternalSystemType>
  <wtg:IsMasterCarton xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:IsMasterCarton>
  <wtg:Receiver xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:Street></wtg:Street>
    <wtg:City></wtg:City>
    <wtg:Region></wtg:Region>
    <wtg:PostalCode></wtg:PostalCode>
    <wtg:Country></wtg:Country>
    <wtg:Residential>false</wtg:Residential>
    <wtg:Modified>false</wtg:Modified>
    <wtg:AccountNumber>AccountNumber2</wtg:AccountNumber>
    <wtg:CompanyName>CompanyName8</wtg:CompanyName>
    <wtg:Locale>Locale0</wtg:Locale>
    <wtg:Other>Other0</wtg:Other>
  </wtg:Receiver>
  <wtg:AutomatePostageMeterAdd xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AutomatePostageMeterAdd>
  <wtg:AutomatePostageMeterRate xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:AutomatePostageMeterRate>
  <wtg:MeterModeShipment xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:MeterModeShipment>
  <wtg:UseCartonization xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:UseCartonization>
  <wtg:Rush xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Rush>
  <wtg:ShipAfterRateResult xmlns:wtg="https://www.wisetechglobal.com/">SuccessOnly</wtg:ShipAfterRateResult>
</wtg:PierbridgeShipRequest>
```

