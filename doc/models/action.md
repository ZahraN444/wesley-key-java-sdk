
# Action

If present, this property tells you what actions you need to take in order for your customer to fulfill a payment using the provided source.

## Structure

`Action`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RedirectUrl` | `String` | Optional | Contains instructions for authenticating a payment by redirecting your customer to another page or application. | String getRedirectUrl() | setRedirectUrl(String redirectUrl) |
| `Type` | `String` | Required | Type of the next action to perform, one of redirect_to_url or use_stripe_sdk. | String getType() | setType(String type) |

## Example (as XML)

```xml
<wtg:Action xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:RedirectUrl xmlns:wtg="https://www.wisetechglobal.com/">RedirectUrl8</wtg:RedirectUrl>
  <wtg:Type xmlns:wtg="https://www.wisetechglobal.com/">Type0</wtg:Type>
</wtg:Action>
```

