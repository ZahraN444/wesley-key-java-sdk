
# BOL Handling

Container to allow handling of BOL to be specified.

## Structure

`BOLHandling`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Email` | `Boolean` | Optional | Specifies whether the BOL should be emailed. Defaults to false if not submitted.<br><br>**Default**: `false` | Boolean getEmail() | setEmail(Boolean email) |
| `EmailAddress` | `String` | Optional | Email address to send the BOL to. | String getEmailAddress() | setEmailAddress(String emailAddress) |

## Example (as XML)

```xml
<wtg:BOLHandling xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Email xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Email>
  <wtg:EmailAddress xmlns:wtg="https://www.wisetechglobal.com/">EmailAddress6</wtg:EmailAddress>
</wtg:BOLHandling>
```

