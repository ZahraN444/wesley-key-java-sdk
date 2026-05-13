
# Packages 11

Container for all packages associated with the transaction.

## Structure

`Packages11`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Package` | [`List<Package12>`](../../doc/models/package-12.md) | Required | Container for an individual package associated with the transaction. | List<Package12> getPackage() | setPackage(List<Package12> mPackage) |

## Example (as XML)

```xml
<wtg:Packages xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:Status></wtg:Status>
    <wtg:Weight>0</wtg:Weight>
    <wtg:PackageType>0</wtg:PackageType>
    <wtg:PackageTypeName>0</wtg:PackageTypeName>
    <wtg:History></wtg:History>
    <wtg:PackageID>56</wtg:PackageID>
    <wtg:WayBillNumber>WayBillNumber6</wtg:WayBillNumber>
    <wtg:ShipperReference>ShipperReference8</wtg:ShipperReference>
  </wtg:Package>
</wtg:Packages>
```

