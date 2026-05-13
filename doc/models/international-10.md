
# International 10

Container for international details associated with the shipment.

## Structure

`International10`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DocumentsOnly` | `Boolean` | Optional | Indicates if the item only contained documents.<br><br>**Default**: `false` | Boolean getDocumentsOnly() | setDocumentsOnly(Boolean documentsOnly) |
| `Contents` | [`Contents8`](../../doc/models/contents-8.md) | Optional | Container for all contents (line items) associated with the transaction. | Contents8 getContents() | setContents(Contents8 contents) |

## Example (as XML)

```xml
<wtg:International xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:DocumentsOnly xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DocumentsOnly>
  <wtg:Contents xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Contents>
</wtg:International>
```

