
# Output Handling

Container to allow handling of outputs to be specified.

## Structure

`OutputHandling`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `EmailOutputs` | `Boolean` | Optional | Specifies whether outputs should be emailed instead of being printed. Defaults to false if not submitted.<br><br>**Default**: `false` | Boolean getEmailOutputs() | setEmailOutputs(Boolean emailOutputs) |
| `EmailAddress` | `String` | Optional | Email address to send the outputs to. | String getEmailAddress() | setEmailAddress(String emailAddress) |

## Example (as XML)

```xml
<wtg:OutputHandling xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:EmailOutputs xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:EmailOutputs>
  <wtg:EmailAddress xmlns:wtg="https://www.wisetechglobal.com/">EmailAddress8</wtg:EmailAddress>
</wtg:OutputHandling>
```

