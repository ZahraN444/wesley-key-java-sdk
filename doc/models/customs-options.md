
# Customs Options

Identifies the customs options for the consolidated shipment.

## Structure

`CustomsOptions`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | `Integer` | Optional | Identifies the customs options type code for the consolidated shipment. | Integer getType() | setType(Integer type) |
| `Description` | `String` | Optional | Identifies the customs options description for the consolidated shipment. | String getDescription() | setDescription(String description) |

## Example (as XML)

```xml
<wtg:CustomsOptions xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Type xmlns:wtg="https://www.wisetechglobal.com/">78</wtg:Type>
  <wtg:Description xmlns:wtg="https://www.wisetechglobal.com/">Description2</wtg:Description>
</wtg:CustomsOptions>
```

