
# Pet

## Structure

`Pet`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `Long` | Optional | - | Long getId() | setId(Long id) |
| `Category` | [`Category2`](../../doc/models/category-2.md) | Optional | - | Category2 getCategory() | setCategory(Category2 category) |
| `Name` | `String` | Required | - | String getName() | setName(String name) |
| `PhotoUrls` | `List<String>` | Required | - | List<String> getPhotoUrls() | setPhotoUrls(List<String> photoUrls) |
| `Tags` | [`List<Tag>`](../../doc/models/tag.md) | Optional | - | List<Tag> getTags() | setTags(List<Tag> tags) |
| `Status` | [`StatusEnum`](../../doc/models/status-enum.md) | Optional | - | StatusEnum getStatus() | setStatus(StatusEnum status) |

## Example (as JSON)

```json
{
  "id": 120,
  "category": null,
  "name": "name0",
  "photoUrls": [
    "photoUrls5",
    "photoUrls6"
  ],
  "tags": [
    null
  ],
  "status": "available"
}
```

