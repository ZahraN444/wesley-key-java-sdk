
# Address

*This model accepts additional fields of type Object.*

## Structure

`Address`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Street` | `String` | Required | - | String getStreet() | setStreet(String street) |
| `City` | `String` | Required | - | String getCity() | setCity(String city) |
| `Zip` | `String` | Optional | - | String getZip() | setZip(String zip) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "street": "123 Main St",
  "city": "New York",
  "zip": "10001",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

