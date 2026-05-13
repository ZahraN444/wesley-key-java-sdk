
# Errors

Container for all errors found whilst processing the transaction.

## Structure

`Errors`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Error` | [`List<Error>`](../../doc/models/error.md) | Optional | Container for a single error found whilst processing the transaction. | List<Error> getError() | setError(List<Error> error) |

## Example (as XML)

```xml
<wtg:Errors xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Error xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Error>
  <wtg:Error xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Error>
  <wtg:Error xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Error>
</wtg:Errors>
```

