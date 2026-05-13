
# Pet

*This model accepts additional fields of type Object.*

## Structure

`Pet`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `Long` | Optional | - | Long getId() | setId(Long id) |
| `Name` | `String` | Required | - | String getName() | setName(String name) |
| `Category` | [`Category`](../../doc/models/category.md) | Optional | - | Category getCategory() | setCategory(Category category) |
| `PhotoUrls` | `List<String>` | Required | - | List<String> getPhotoUrls() | setPhotoUrls(List<String> photoUrls) |
| `Tags` | [`List<Tag>`](../../doc/models/tag.md) | Optional | - | List<Tag> getTags() | setTags(List<Tag> tags) |
| `Status` | [`PetStatus`](../../doc/models/pet-status.md) | Optional | pet status in the store | PetStatus getStatus() | setStatus(PetStatus status) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "id": 120,
  "name": "name0",
  "category": {
    "id": 232,
    "name": "name2",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "photoUrls": [
    "photoUrls5",
    "photoUrls6"
  ],
  "tags": [
    {
      "id": 26,
      "name": "name0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "status": "available",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

