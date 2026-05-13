
# International 2

Container for international details associated with the shipment.

## Structure

`International2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DocumentsOnly` | `Boolean` | Optional | Indicates if the item only contained documents.<br><br>**Default**: `false` | Boolean getDocumentsOnly() | setDocumentsOnly(Boolean documentsOnly) |
| `Contents` | [`Contents2`](../../doc/models/contents-2.md) | Optional | Container for all contents (line items) associated with the transaction. | Contents2 getContents() | setContents(Contents2 contents) |

## Example (as XML)

```xml
<wtg:International xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:DocumentsOnly xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DocumentsOnly>
  <wtg:Contents xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Contents>
</wtg:International>
```

