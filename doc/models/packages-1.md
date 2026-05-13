
# Packages 1

Container for all packages associated with the transaction.

## Structure

`Packages1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Package` | [`List<Package1>`](../../doc/models/package-1.md) | Required | Container for an individual package associated with the transaction. | List<Package1> getPackage() | setPackage(List<Package1> mPackage) |

## Example (as XML)

```xml
<wtg:Packages xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:Status></wtg:Status>
    <wtg:AdditionalHandling>false</wtg:AdditionalHandling>
    <wtg:Oversize>0</wtg:Oversize>
    <wtg:PackageType>0</wtg:PackageType>
    <wtg:Weight>0</wtg:Weight>
    <wtg:ISOCurrencyId>0</wtg:ISOCurrencyId>
    <wtg:PackageID>0</wtg:PackageID>
    <wtg:RecordIdentifiers></wtg:RecordIdentifiers>
    <wtg:FreightClass>FreightClass6</wtg:FreightClass>
  </wtg:Package>
</wtg:Packages>
```

