
# Documents 1

Container for documents to be printed by the caller of the transaction (client).

## Structure

`Documents1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Output` | [`List<Output3>`](../../doc/models/output-3.md) | Optional | Container for documents to be printed externally from the transaction. | List<Output3> getOutput() | setOutput(List<Output3> output) |

## Example (as XML)

```xml
<wtg:Documents xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Output xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Output>
</wtg:Documents>
```

