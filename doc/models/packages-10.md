
# Packages 10

Container for all packages associated with the transaction.

## Structure

`Packages10`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Package` | [`List<Package11>`](../../doc/models/package-11.md) | Required | Container for an individual package associated with the transaction. | List<Package11> getPackage() | setPackage(List<Package11> mPackage) |

## Example (as XML)

```xml
<wtg:Packages xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:AccountID>0</wtg:AccountID>
    <wtg:PackageID>0</wtg:PackageID>
    <wtg:WayBillNumber>WayBillNumber6</wtg:WayBillNumber>
    <wtg:ShipperReference>ShipperReference8</wtg:ShipperReference>
    <wtg:ReferenceOne>ReferenceOne8</wtg:ReferenceOne>
  </wtg:Package>
</wtg:Packages>
```

