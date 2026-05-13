
# Status

Container for transaction errors and warning elements.

## Structure

`Status`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Code` | `int` | Required | If the transaction was successful this was will equal one, otherwise zero. | int getCode() | setCode(int code) |
| `Description` | `String` | Optional | Contains a description of the status, if the transaction failed this will contain an error message. | String getDescription() | setDescription(String description) |
| `Warnings` | [`Warnings`](../../doc/models/warnings.md) | Optional | Container for all warnings found whilst processing the transaction. | Warnings getWarnings() | setWarnings(Warnings warnings) |
| `Errors` | [`Errors`](../../doc/models/errors.md) | Optional | Container for all errors found whilst processing the transaction. | Errors getErrors() | setErrors(Errors errors) |

## Example (as XML)

```xml
<wtg:Status xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Code xmlns:wtg="https://www.wisetechglobal.com/">108</wtg:Code>
  <wtg:Description xmlns:wtg="https://www.wisetechglobal.com/">Description8</wtg:Description>
  <wtg:Warnings xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Warnings>
  <wtg:Errors xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Errors>
</wtg:Status>
```

