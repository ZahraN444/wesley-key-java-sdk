
# International 1

Container for international details associated with the shipment.

## Structure

`International1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `IsInternational` | `Boolean` | Optional | Indicates whether the package is part of an international shipment.  Defaults to no if omitted.<br><br>**Default**: `false` | Boolean getIsInternational() | setIsInternational(Boolean isInternational) |
| `NonDutiable` | `Boolean` | Optional | Indicates whether the package contains only non-dutiable goods.  Defaults to no if omitted.<br><br>**Default**: `false` | Boolean getNonDutiable() | setNonDutiable(Boolean nonDutiable) |
| `DocumentsOnly` | `Boolean` | Optional | Indicates whether the package contains only documents.  Defaults to not documents only if omitted.<br><br>**Default**: `false` | Boolean getDocumentsOnly() | setDocumentsOnly(Boolean documentsOnly) |
| `PrePackedBoxes` | [`PrePackedBoxes`](../../doc/models/pre-packed-boxes.md) | Optional | pre-packed boxes, including any items specified that will be packed and excess space used before any new boxes are created. | PrePackedBoxes getPrePackedBoxes() | setPrePackedBoxes(PrePackedBoxes prePackedBoxes) |
| `Contents` | [`Contents`](../../doc/models/contents.md) | Optional | Container for all contents (line items) associated with the transaction. | Contents getContents() | setContents(Contents contents) |

## Example (as XML)

```xml
<wtg:International xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:IsInternational xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:IsInternational>
  <wtg:NonDutiable xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:NonDutiable>
  <wtg:DocumentsOnly xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:DocumentsOnly>
  <wtg:PrePackedBoxes xmlns:wtg="https://www.wisetechglobal.com/"></wtg:PrePackedBoxes>
  <wtg:Contents xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Contents>
</wtg:International>
```

