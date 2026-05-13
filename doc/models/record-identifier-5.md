
# Record Identifier 5

Inner container for transaction identifiers.

## Structure

`RecordIdentifier5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RecordIdentifierID` | `Integer` | Optional | The unique numeric identifier for the Key1 through Key6 record.<br><br>**Default**: `0` | Integer getRecordIdentifierID() | setRecordIdentifierID(Integer recordIdentifierID) |
| `Keys` | [`Keys`](../../doc/models/keys.md) | Optional | Container for transaction identifiers to be stored. | Keys getKeys() | setKeys(Keys keys) |

## Example (as XML)

```xml
<wtg:RecordIdentifier xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:RecordIdentifierID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:RecordIdentifierID>
  <wtg:Keys xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Keys>
</wtg:RecordIdentifier>
```

