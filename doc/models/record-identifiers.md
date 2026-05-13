
# Record Identifiers

Outer container for transaction identifiers.

## Structure

`RecordIdentifiers`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RecordIdentifier` | [`List<RecordIdentifier>`](../../doc/models/record-identifier.md) | Optional | Inner container for transaction identifiers. | List<RecordIdentifier> getRecordIdentifier() | setRecordIdentifier(List<RecordIdentifier> recordIdentifier) |

## Example (as XML)

```xml
<wtg:RecordIdentifiers xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:RecordIdentifier xmlns:wtg="https://www.wisetechglobal.com/"></wtg:RecordIdentifier>
  <wtg:RecordIdentifier xmlns:wtg="https://www.wisetechglobal.com/"></wtg:RecordIdentifier>
</wtg:RecordIdentifiers>
```

