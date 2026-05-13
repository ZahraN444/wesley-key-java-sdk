
# Pages

Container for all pages to be printed by the caller of the transaction (client).

## Structure

`Pages`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Page` | [`List<Page>`](../../doc/models/page.md) | Optional | Container for an individual page to be printed by the caller of the transaction (client). | List<Page> getPage() | setPage(List<Page> page) |

## Example (as XML)

```xml
<wtg:Pages xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Page xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Page>
  <wtg:Page xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Page>
</wtg:Pages>
```

