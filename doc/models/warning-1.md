
# Warning 1

Container for a single warning found whilst processing the transaction.

## Structure

`Warning1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Code` | `int` | Required | A code indicating the warning status. | int getCode() | setCode(int code) |
| `Description` | `String` | Required | A description of the warning. | String getDescription() | setDescription(String description) |

## Example (as XML)

```xml
<wtg:Warning xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Code xmlns:wtg="https://www.wisetechglobal.com/">230</wtg:Code>
  <wtg:Description xmlns:wtg="https://www.wisetechglobal.com/">Description0</wtg:Description>
</wtg:Warning>
```

