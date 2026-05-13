
# Order

*This model accepts additional fields of type Object.*

## Structure

`Order`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `Long` | Optional | - | Long getId() | setId(Long id) |
| `PetId` | `Long` | Optional | - | Long getPetId() | setPetId(Long petId) |
| `Quantity` | `Integer` | Optional | - | Integer getQuantity() | setQuantity(Integer quantity) |
| `ShipDate` | `LocalDateTime` | Optional | - | LocalDateTime getShipDate() | setShipDate(LocalDateTime shipDate) |
| `Status` | [`OrderStatus`](../../doc/models/order-status.md) | Optional | Order Status | OrderStatus getStatus() | setStatus(OrderStatus status) |
| `Complete` | `Boolean` | Optional | - | Boolean getComplete() | setComplete(Boolean complete) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "id": 180,
  "petId": 220,
  "quantity": 136,
  "shipDate": "2016-03-13T12:52:32.123Z",
  "status": "placed",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

