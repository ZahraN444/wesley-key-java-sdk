
# Packages 13

Container for all packages associated with the transaction.

## Structure

`Packages13`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Package` | [`List<Package14>`](../../doc/models/package-14.md) | Required | Container for an individual package associated with the transaction. | List<Package14> getPackage() | setPackage(List<Package14> mPackage) |

## Example (as XML)

```xml
<wtg:Packages xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:PackageID>0</wtg:PackageID>
    <wtg:PackageHistoryState>0</wtg:PackageHistoryState>
    <wtg:Status></wtg:Status>
    <wtg:ShipperReference>ShipperReference8</wtg:ShipperReference>
    <wtg:ReferenceOne>ReferenceOne8</wtg:ReferenceOne>
    <wtg:ReferenceTwo>ReferenceTwo4</wtg:ReferenceTwo>
  </wtg:Package>
</wtg:Packages>
```

