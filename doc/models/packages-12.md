
# Packages 12

Container for all packages associated with the transaction.

## Structure

`Packages12`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Package` | [`List<Package13>`](../../doc/models/package-13.md) | Required | Container for an individual package associated with the transaction. | List<Package13> getPackage() | setPackage(List<Package13> mPackage) |

## Example (as XML)

```xml
<wtg:Packages xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:PackageID>0</wtg:PackageID>
    <wtg:WayBillNumber>WayBillNumber6</wtg:WayBillNumber>
  </wtg:Package>
</wtg:Packages>
```

