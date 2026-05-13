
# International 12

Container for international details associated with the shipment.

## Structure

`International12`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DocumentsOnly` | `Boolean` | Optional | Indicates if the item only contained documents.<br><br>**Default**: `false` | Boolean getDocumentsOnly() | setDocumentsOnly(Boolean documentsOnly) |
| `Contents` | [`Contents10`](../../doc/models/contents-10.md) | Optional | Container for all contents (line items) associated with the transaction. | Contents10 getContents() | setContents(Contents10 contents) |

## Example (as XML)

```xml
<wtg:International xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:DocumentsOnly xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DocumentsOnly>
  <wtg:Contents xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Contents>
</wtg:International>
```

