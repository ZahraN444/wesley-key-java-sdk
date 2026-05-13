
# Warnings

Container for all warnings found whilst processing the transaction.

## Structure

`Warnings`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Warning` | [`List<Warning>`](../../doc/models/warning.md) | Optional | Container for a single warning found whilst processing the transaction. | List<Warning> getWarning() | setWarning(List<Warning> warning) |

## Example (as XML)

```xml
<wtg:Warnings xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Warning xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Warning>
  <wtg:Warning xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Warning>
  <wtg:Warning xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Warning>
</wtg:Warnings>
```

