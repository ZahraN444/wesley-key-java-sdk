
# Webhook Update

*This model accepts additional fields of type Object.*

## Structure

`WebhookUpdate`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Url` | `String` | Optional | - | String getUrl() | setUrl(String url) |
| `Events` | `List<String>` | Optional | - | List<String> getEvents() | setEvents(List<String> events) |
| `Secret` | `String` | Optional | - | String getSecret() | setSecret(String secret) |
| `Active` | `Boolean` | Optional | - | Boolean getActive() | setActive(Boolean active) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "url": "url6",
  "events": [
    "events8",
    "events9"
  ],
  "secret": "secret2",
  "active": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

