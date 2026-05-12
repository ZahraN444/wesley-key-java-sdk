
# Order Item

*This model accepts additional fields of type Object.*

## Structure

`OrderItem`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ProductId` | `String` | Required | - | String getProductId() | setProductId(String productId) |
| `Quantity` | `int` | Required | **Constraints**: `>= 1` | int getQuantity() | setQuantity(int quantity) |
| `Price` | `double` | Required | **Constraints**: `>= 0` | double getPrice() | setPrice(double price) |
| `Description` | `String` | Optional | - | String getDescription() | setDescription(String description) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "productId": "prod_001",
  "quantity": 2,
  "price": 29.99,
  "description": "Premium Widget",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

