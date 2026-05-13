
# Documents

Container for documents to be printed by the caller of the transaction (client).

## Structure

`Documents`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Output` | [`List<Output2>`](../../doc/models/output-2.md) | Optional | Container for documents to be printed externally from the transaction. | List<Output2> getOutput() | setOutput(List<Output2> output) |

## Example (as XML)

```xml
<wtg:Documents xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Output xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Output>
  <wtg:Output xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Output>
</wtg:Documents>
```

