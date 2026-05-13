
# Packages 9

Container for all packages associated with the transaction.

## Structure

`Packages9`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Package` | [`List<Package10>`](../../doc/models/package-10.md) | Required | Container for an individual package associated with the transaction. | List<Package10> getPackage() | setPackage(List<Package10> mPackage) |

## Example (as XML)

```xml
<wtg:Packages xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:CartonID>0</wtg:CartonID>
    <wtg:Copies>0</wtg:Copies>
    <wtg:PackageRequisitionID>0</wtg:PackageRequisitionID>
    <wtg:PackItemID>0</wtg:PackItemID>
    <wtg:PackageID>0</wtg:PackageID>
    <wtg:PackageType>0</wtg:PackageType>
    <wtg:Weight>0</wtg:Weight>
    <wtg:MajorWeight>0</wtg:MajorWeight>
    <wtg:MinorWeight>0</wtg:MinorWeight>
    <wtg:Length>0</wtg:Length>
    <wtg:Width>0</wtg:Width>
    <wtg:Height>0</wtg:Height>
    <wtg:Cubic>0</wtg:Cubic>
    <wtg:Linear>0</wtg:Linear>
    <wtg:PriorityAlert>false</wtg:PriorityAlert>
    <wtg:PriorityAlertPlus>false</wtg:PriorityAlertPlus>
    <wtg:InsideDelivery>false</wtg:InsideDelivery>
    <wtg:GuaranteedService>0</wtg:GuaranteedService>
    <wtg:ECOD>false</wtg:ECOD>
    <wtg:Hold>false</wtg:Hold>
    <wtg:HazardousPackagingQuantity>0</wtg:HazardousPackagingQuantity>
    <wtg:AdditionalHandling>false</wtg:AdditionalHandling>
    <wtg:LargePackage>false</wtg:LargePackage>
    <wtg:DeliveryConfirmation>0</wtg:DeliveryConfirmation>
    <wtg:VerbalConfirmation>false</wtg:VerbalConfirmation>
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
    <wtg:Name>Name4</wtg:Name>
    <wtg:RecordIdentifiers></wtg:RecordIdentifiers>
    <wtg:ExternalTrackingID>ExternalTrackingID6</wtg:ExternalTrackingID>
  </wtg:Package>
</wtg:Packages>
```

