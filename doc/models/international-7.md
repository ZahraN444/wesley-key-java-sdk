
# International 7

Container for international details associated with the shipment.

## Structure

`International7`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DocumentsOnly` | `boolean` | Required | Indicates if the item only contained documents. | boolean getDocumentsOnly() | setDocumentsOnly(boolean documentsOnly) |

## Example (as XML)

```xml
<wtg:International xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:DocumentsOnly xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DocumentsOnly>
</wtg:International>
```

