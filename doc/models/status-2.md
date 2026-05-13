
# Status 2

Container for HubCapp printing status.

## Structure

`Status2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Code` | `Integer` | Optional | If the transaction was successful this was will equal one, otherwise zero. | Integer getCode() | setCode(Integer code) |
| `Description` | `String` | Optional | Contains a description of the status, if the transaction failed this will contain an error message. | String getDescription() | setDescription(String description) |

## Example (as XML)

```xml
<wtg:Status xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Code xmlns:wtg="https://www.wisetechglobal.com/">28</wtg:Code>
  <wtg:Description xmlns:wtg="https://www.wisetechglobal.com/">Description4</wtg:Description>
</wtg:Status>
```

