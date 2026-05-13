
# International 6

Container for international details associated with the shipment.

## Structure

`International6`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Contents` | [`Contents5`](../../doc/models/contents-5.md) | Optional | Container for all contents (line items) associated with the transaction. | Contents5 getContents() | setContents(Contents5 contents) |

## Example (as XML)

```xml
<wtg:International xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Contents xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Contents>
</wtg:International>
```

