
# Cartonization

Container for cartonization data for this transaction.

## Structure

`Cartonization`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Carrier` | `String` | Optional | The id of the carrier to use for cartonization. | String getCarrier() | setCarrier(String carrier) |
| `UserName` | `String` | Optional | The username to use for the underlying cartonization request. | String getUserName() | setUserName(String userName) |
| `ControlIdentifier` | `String` | Optional | The control identifier to use for the underlying cartonization request. | String getControlIdentifier() | setControlIdentifier(String controlIdentifier) |
| `DimensionsUOM` | `String` | Optional | The units of measure for the box length, width and height. | String getDimensionsUOM() | setDimensionsUOM(String dimensionsUOM) |
| `WeightUOM` | `String` | Optional | The units of measure for the unit weight. | String getWeightUOM() | setWeightUOM(String weightUOM) |
| `CurrencyCode` | `String` | Optional | Currency of the value of the comtent. | String getCurrencyCode() | setCurrencyCode(String currencyCode) |
| `LayFlat` | `Boolean` | Optional | Aligns all items laying flat. If possible, it may create a "brick-laying" pattern to increase stability. | Boolean getLayFlat() | setLayFlat(Boolean layFlat) |
| `Corners` | `Boolean` | Optional | Only pack items at valid corner points of other items (optimal) | Boolean getCorners() | setCorners(Boolean corners) |
| `UsableSpace` | `Double` | Optional | Estimate of percentage space in boxes that is usable, i.e., not packing material. | Double getUsableSpace() | setUsableSpace(Double usableSpace) |
| `ReservedSpace` | `Double` | Optional | Space in boxes that is reserved, i.e., for packing material.. | Double getReservedSpace() | setReservedSpace(Double reservedSpace) |
| `BoxTypeChoiceGoal` | `String` | Optional | The objective to evaluate boxTypeChoices by. ‘lowest-cost’ minimizes price or volume cost of boxTypes selected, ‘most-items’ maximizes item count per box opened, i.e., fewest total boxes used. | String getBoxTypeChoiceGoal() | setBoxTypeChoiceGoal(String boxTypeChoiceGoal) |
| `BoxTypeSets` | [`BoxTypeSets`](../../doc/models/box-type-sets.md) | Optional | predefined box types to be used, separated by commas. Will be overridden by boxTypes. | BoxTypeSets getBoxTypeSets() | setBoxTypeSets(BoxTypeSets boxTypeSets) |
| `Rules` | `String` | Optional | a space-delimited array of packing rule strings. The only acceptable rule-type at the moment is "exclude", and it follows the form; exclude,[item-ref-id],[target-item-ref-id] | String getRules() | setRules(String rules) |
| `CartonizationGroupID` | `int` | Required | Numeric identifier for a cartonization group.<br><br>**Default**: `0` | int getCartonizationGroupID() | setCartonizationGroupID(int cartonizationGroupID) |
| `Contents` | [`Contents1`](../../doc/models/contents-1.md) | Required | Container for all contents associated with the transaction. | Contents1 getContents() | setContents(Contents1 contents) |
| `PackageTemplate` | [`PackageTemplate`](../../doc/models/package-template.md) | Required | Container for elements to be applied to each package created from the cartonization response . | PackageTemplate getPackageTemplate() | setPackageTemplate(PackageTemplate packageTemplate) |

## Example (as XML)

```xml
<wtg:Cartonization xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:CartonizationGroupID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:CartonizationGroupID>
  <wtg:Contents xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:Content></wtg:Content>
  </wtg:Contents>
  <wtg:PackageTemplate xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:Copies>0</wtg:Copies>
    <wtg:PackageRequisitionID>0</wtg:PackageRequisitionID>
    <wtg:PackItemID>0</wtg:PackItemID>
    <wtg:PriorityAlert>false</wtg:PriorityAlert>
    <wtg:PriorityAlertPlus>false</wtg:PriorityAlertPlus>
    <wtg:GuaranteedService>0</wtg:GuaranteedService>
    <wtg:ECOD>false</wtg:ECOD>
    <wtg:Hold>false</wtg:Hold>
    <wtg:HazardousPackagingQuantity>0</wtg:HazardousPackagingQuantity>
    <wtg:AdditionalHandling>false</wtg:AdditionalHandling>
    <wtg:LargePackage>false</wtg:LargePackage>
    <wtg:ContainerType>0</wtg:ContainerType>
    <wtg:ExcessiveLengthType>0</wtg:ExcessiveLengthType>
    <wtg:VerbalConfirmation>false</wtg:VerbalConfirmation>
    <wtg:PalletCount>0</wtg:PalletCount>
    <wtg:ItemsOnPallet>0</wtg:ItemsOnPallet>
    <wtg:NonStandardContainer>false</wtg:NonStandardContainer>
    <wtg:EmailNotification>false</wtg:EmailNotification>
    <wtg:NonFlatMachinable>false</wtg:NonFlatMachinable>
    <wtg:NonMachinable>false</wtg:NonMachinable>
    <wtg:NonRectangular>false</wtg:NonRectangular>
    <wtg:Flat>false</wtg:Flat>
    <wtg:Registered>false</wtg:Registered>
    <wtg:RestrictedDelivery>false</wtg:RestrictedDelivery>
    <wtg:ReturnReceipt>false</wtg:ReturnReceipt>
    <wtg:Certified>false</wtg:Certified>
    <wtg:DryIceWeight>0</wtg:DryIceWeight>
    <wtg:ERR>false</wtg:ERR>
    <wtg:ReturnReceiptMerchandise>false</wtg:ReturnReceiptMerchandise>
    <wtg:ElectronicCertified>false</wtg:ElectronicCertified>
    <wtg:Exchange>false</wtg:Exchange>
    <wtg:ExternalTrackingID>ExternalTrackingID6</wtg:ExternalTrackingID>
    <wtg:ShipperReference>ShipperReference8</wtg:ShipperReference>
  </wtg:PackageTemplate>
  <wtg:Carrier xmlns:wtg="https://www.wisetechglobal.com/">Carrier2</wtg:Carrier>
  <wtg:UserName xmlns:wtg="https://www.wisetechglobal.com/">UserName2</wtg:UserName>
  <wtg:ControlIdentifier xmlns:wtg="https://www.wisetechglobal.com/">ControlIdentifier4</wtg:ControlIdentifier>
  <wtg:DimensionsUOM xmlns:wtg="https://www.wisetechglobal.com/">DimensionsUOM0</wtg:DimensionsUOM>
  <wtg:WeightUOM xmlns:wtg="https://www.wisetechglobal.com/">WeightUOM6</wtg:WeightUOM>
</wtg:Cartonization>
```

