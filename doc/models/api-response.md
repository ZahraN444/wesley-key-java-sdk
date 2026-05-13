
# Api Response

*This model accepts additional fields of type Object.*

## Structure

`ApiResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Code` | `Integer` | Optional | - | Integer getCode() | setCode(Integer code) |
| `Type` | `String` | Optional | - | String getType() | setType(String type) |
| `Message` | `String` | Optional | - | String getMessage() | setMessage(String message) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "code": 142,
  "type": "type0",
  "message": "message0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

