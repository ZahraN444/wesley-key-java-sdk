
# Delivery Details

*This model accepts additional fields of type Object.*

## Structure

`DeliveryDetails`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Method` | `String` | Optional | - | String getMethod() | setMethod(String method) |
| `Eta` | `LocalDateTime` | Optional | - | LocalDateTime getEta() | setEta(LocalDateTime eta) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "method": "method6",
  "eta": "2016-03-13T12:52:32.123Z",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

