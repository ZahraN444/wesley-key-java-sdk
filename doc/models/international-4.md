
# International 4

Container for international details associated with the shipment.

## Structure

`International4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `NonDutiable` | `Boolean` | Optional | Indicates whether the package contains only non-dutiable goods.  Defaults to no if omitted.<br><br>**Default**: `false` | Boolean getNonDutiable() | setNonDutiable(Boolean nonDutiable) |
| `DocumentsOnly` | `Boolean` | Optional | Indicates whether the package contains only documents.  Defaults to not documents only if omitted.<br><br>**Default**: `false` | Boolean getDocumentsOnly() | setDocumentsOnly(Boolean documentsOnly) |
| `Contents` | [`Contents4`](../../doc/models/contents-4.md) | Optional | Container for all contents (line items) associated with the transaction. | Contents4 getContents() | setContents(Contents4 contents) |

## Example (as XML)

```xml
<wtg:International xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:NonDutiable xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NonDutiable>
  <wtg:DocumentsOnly xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DocumentsOnly>
  <wtg:Contents xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Contents>
</wtg:International>
```

