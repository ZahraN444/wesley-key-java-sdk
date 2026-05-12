
# Webhook Registration

*This model accepts additional fields of type Object.*

## Structure

`WebhookRegistration`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Url` | `String` | Required | The endpoint URL that will receive webhook events | String getUrl() | setUrl(String url) |
| `Events` | [`List<Event>`](../../doc/models/event.md) | Required | List of events to subscribe to | List<Event> getEvents() | setEvents(List<Event> events) |
| `Secret` | `String` | Optional | Secret key for webhook signature verification | String getSecret() | setSecret(String secret) |
| `Active` | `Boolean` | Optional | Whether the webhook is active<br><br>**Default**: `true` | Boolean getActive() | setActive(Boolean active) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "url": "https://merchant.example.com/webhooks/events",
  "events": [
    "order.created",
    "payment.completed"
  ],
  "secret": "webhook_secret_key_123",
  "active": true,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

