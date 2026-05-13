
# Record Identifier 1

Inner container for transaction identifiers.

## Structure

`RecordIdentifier1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RecordIdentifierID` | `int` | Required | Unique identifier for the record identifier record. | int getRecordIdentifierID() | setRecordIdentifierID(int recordIdentifierID) |
| `Keys` | [`Keys`](../../doc/models/keys.md) | Optional | Container for transaction identifiers to be stored. | Keys getKeys() | setKeys(Keys keys) |

## Example (as XML)

```xml
<wtg:RecordIdentifier xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:RecordIdentifierID xmlns:wtg="https://www.wisetechglobal.com/">124</wtg:RecordIdentifierID>
  <wtg:Keys xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Keys>
</wtg:RecordIdentifier>
```

