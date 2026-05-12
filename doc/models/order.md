
# Order

*This model accepts additional fields of type Object.*

## Structure

`Order`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `OrderId` | `String` | Optional | - | String getOrderId() | setOrderId(String orderId) |
| `CustomerId` | `String` | Optional | - | String getCustomerId() | setCustomerId(String customerId) |
| `Items` | [`List<OrderItem>`](../../doc/models/order-item.md) | Optional | - | List<OrderItem> getItems() | setItems(List<OrderItem> items) |
| `TotalAmount` | `Double` | Optional | - | Double getTotalAmount() | setTotalAmount(Double totalAmount) |
| `Status` | [`Status`](../../doc/models/status.md) | Optional | - | Status getStatus() | setStatus(Status status) |
| `CreatedAt` | `LocalDateTime` | Optional | - | LocalDateTime getCreatedAt() | setCreatedAt(LocalDateTime createdAt) |
| `UpdatedAt` | `LocalDateTime` | Optional | - | LocalDateTime getUpdatedAt() | setUpdatedAt(LocalDateTime updatedAt) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "orderId": "order_789",
  "customerId": "cust_12345",
  "totalAmount": 59.98,
  "status": "pending",
  "createdAt": "09/19/2025 10:30:00",
  "updatedAt": "09/19/2025 10:30:00",
  "items": [
    {
      "productId": "productId2",
      "quantity": 22,
      "price": 56.94,
      "description": "description2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

