
# International 3

Container for international details associated with the shipment.

## Structure

`International3`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Contents` | [`Contents3`](../../doc/models/contents-3.md) | Optional | Container for all contents (line items) associated with the transaction. | Contents3 getContents() | setContents(Contents3 contents) |

## Example (as XML)

```xml
<wtg:International xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Contents xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Contents>
</wtg:International>
```

