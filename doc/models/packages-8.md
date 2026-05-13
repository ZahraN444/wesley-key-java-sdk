
# Packages 8

Container for all packages associated with the transaction.

## Structure

`Packages8`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Package` | [`List<Package9>`](../../doc/models/package-9.md) | Required | Container for an individual package associated with the transaction. | List<Package9> getPackage() | setPackage(List<Package9> mPackage) |

## Example (as XML)

```xml
<wtg:Packages xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:Status></wtg:Status>
    <wtg:AdditionalHandling>false</wtg:AdditionalHandling>
    <wtg:Oversize>0</wtg:Oversize>
    <wtg:PackageType>0</wtg:PackageType>
    <wtg:Weight>0</wtg:Weight>
    <wtg:ShipToHoldState>0</wtg:ShipToHoldState>
    <wtg:RecordIdentifiers></wtg:RecordIdentifiers>
    <wtg:MailPieceNumber>MailPieceNumber2</wtg:MailPieceNumber>
    <wtg:UniqueIdentifier>UniqueIdentifier0</wtg:UniqueIdentifier>
    <wtg:OtherIdentifier>OtherIdentifier2</wtg:OtherIdentifier>
    <wtg:BillingCode>BillingCode6</wtg:BillingCode>
  </wtg:Package>
</wtg:Packages>
```

