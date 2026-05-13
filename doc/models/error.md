
# Error

Container for a single error found whilst processing the transaction.

## Structure

`Error`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Code` | `Integer` | Optional | A code indicating the error status.<br><br>**Default**: `0` | Integer getCode() | setCode(Integer code) |
| `Description` | `String` | Required | A description of the error. | String getDescription() | setDescription(String description) |

## Example (as XML)

```xml
<wtg:Error xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Code xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Code>
  <wtg:Description xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Description>
</wtg:Error>
```

