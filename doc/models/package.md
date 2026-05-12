
# Package

*This model accepts additional fields of type Object.*

## Structure

`Package`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PackageId` | `String` | Optional | - | String getPackageId() | setPackageId(String packageId) |
| `Weight` | `Double` | Optional | - | Double getWeight() | setWeight(Double weight) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "packageId": "packageId0",
  "weight": 83.8,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

