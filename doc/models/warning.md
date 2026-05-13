
# Warning

Container for a single warning found whilst processing the transaction.

## Structure

`Warning`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Code` | `Integer` | Optional | A code indicating the warning status.<br><br>**Default**: `0` | Integer getCode() | setCode(Integer code) |
| `Description` | `String` | Required | A description of the warning. | String getDescription() | setDescription(String description) |

## Example (as XML)

```xml
<wtg:Warning xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Code xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Code>
  <wtg:Description xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Description>
</wtg:Warning>
```

