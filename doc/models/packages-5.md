
# Packages 5

Container for all packages associated with the transaction.

## Structure

`Packages5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Package` | [`List<Package6>`](../../doc/models/package-6.md) | Required | Container for an individual package associated with the transaction. | List<Package6> getPackage() | setPackage(List<Package6> mPackage) |

## Example (as XML)

```xml
<wtg:Packages xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:Status></wtg:Status>
    <wtg:AdditionalHandling>false</wtg:AdditionalHandling>
    <wtg:Oversize>0</wtg:Oversize>
    <wtg:PackageType>0</wtg:PackageType>
    <wtg:FreightClass>FreightClass6</wtg:FreightClass>
    <wtg:ShipperReference>ShipperReference8</wtg:ShipperReference>
  </wtg:Package>
</wtg:Packages>
```

