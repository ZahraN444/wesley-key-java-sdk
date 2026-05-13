
# Labels

Container for labels to be printed by the caller of the transaction (client).

## Structure

`Labels`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Output` | [`List<Output1>`](../../doc/models/output-1.md) | Optional | Container for labels to be printed externally from the transaction. | List<Output1> getOutput() | setOutput(List<Output1> output) |

## Example (as XML)

```xml
<wtg:Labels xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Output xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Output>
  <wtg:Output xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Output>
  <wtg:Output xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Output>
</wtg:Labels>
```

