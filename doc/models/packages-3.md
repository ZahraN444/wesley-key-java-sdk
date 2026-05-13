
# Packages 3

Container for all packages associated with the transaction.

## Structure

`Packages3`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Package` | [`List<Package3>`](../../doc/models/package-3.md) | Required | Container for an individual package associated with the transaction. | List<Package3> getPackage() | setPackage(List<Package3> mPackage) |

## Example (as XML)

```xml
<wtg:Packages xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:ProactiveResponse>false</wtg:ProactiveResponse>
    <wtg:LithiumBattery>false</wtg:LithiumBattery>
    <wtg:Copies>0</wtg:Copies>
    <wtg:PackageRequisitionID>0</wtg:PackageRequisitionID>
    <wtg:PackItemID>0</wtg:PackItemID>
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
    <wtg:GuaranteedService>0</wtg:GuaranteedService>
    <wtg:ECOD>false</wtg:ECOD>
    <wtg:HoldDeliveryType>DeliverDirectToHoldLocation</wtg:HoldDeliveryType>
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
    <wtg:LooseDryIce>false</wtg:LooseDryIce>
    <wtg:ERR>false</wtg:ERR>
    <wtg:ReturnReceiptMerchandise>false</wtg:ReturnReceiptMerchandise>
    <wtg:ElectronicCertified>false</wtg:ElectronicCertified>
    <wtg:Exchange>false</wtg:Exchange>
    <wtg:SpecialCare></wtg:SpecialCare>
    <wtg:LithiumBatteryDetails></wtg:LithiumBatteryDetails>
  </wtg:Package>
</wtg:Packages>
```

