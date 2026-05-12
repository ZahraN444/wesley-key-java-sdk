
# Error Exception

*This model accepts additional fields of type Object.*

## Structure

`ErrorException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Error` | `String` | Required | Error code | String getError() | setError(String error) |
| `Message` | `String` | Required | Human-readable error message | String getMessageField() | setMessageField(String messageField) |
| `Details` | `Object` | Optional | Additional error details | Object getDetails() | setDetails(Object details) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "error": "invalid_request",
  "message": "The request body is invalid",
  "details": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

