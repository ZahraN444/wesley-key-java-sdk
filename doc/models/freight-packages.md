
# Freight Packages

Container for all packages associated with the transaction.

## Structure

`FreightPackages`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Package` | [`List<Package5>`](../../doc/models/package-5.md) | Required | Container for an individual package associated with the transaction. | List<Package5> getPackage() | setPackage(List<Package5> mPackage) |

## Example (as XML)

```xml
<wtg:FreightPackages xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:Weight>0</wtg:Weight>
    <wtg:Length>0</wtg:Length>
    <wtg:Width>0</wtg:Width>
    <wtg:Height>0</wtg:Height>
    <wtg:PalletCount>0</wtg:PalletCount>
    <wtg:ItemsOnPallet>0</wtg:ItemsOnPallet>
    <wtg:FreightClass>FreightClass6</wtg:FreightClass>
  </wtg:Package>
</wtg:FreightPackages>
```

