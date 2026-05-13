
# Identification

Container for client identification elements.

## Structure

`Identification`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `WorkstationIdentifier` | `String` | Required | Unique identifier for the workstation that submitted the request, this node is automatically added if needed. | String getWorkstationIdentifier() | setWorkstationIdentifier(String workstationIdentifier) |
| `RequestUserIdentifier` | `String` | Optional | The underlying username that submitted the request, this node is automatically added if needed. | String getRequestUserIdentifier() | setRequestUserIdentifier(String requestUserIdentifier) |

## Example (as XML)

```xml
<wtg:Identification xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:WorkstationIdentifier xmlns:wtg="https://www.wisetechglobal.com/">WorkstationIdentifier0</wtg:WorkstationIdentifier>
  <wtg:RequestUserIdentifier xmlns:wtg="https://www.wisetechglobal.com/">RequestUserIdentifier6</wtg:RequestUserIdentifier>
</wtg:Identification>
```

