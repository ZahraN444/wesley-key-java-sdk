
# Create Order Request

*This model accepts additional fields of type Object.*

## Structure

`CreateOrderRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `CustomerId` | `String` | Required | Unique identifier for the customer | String getCustomerId() | setCustomerId(String customerId) |
| `Items` | [`List<OrderItem>`](../../doc/models/order-item.md) | Required | **Constraints**: *Minimum Items*: `1` | List<OrderItem> getItems() | setItems(List<OrderItem> items) |
| `CallbackUrl` | `String` | Required | URL to receive callback notifications | String getCallbackUrl() | setCallbackUrl(String callbackUrl) |
| `Document` | `InputStream` | Optional | Binary file upload | InputStream getDocument() | setDocument(InputStream document) |
| `Metadata` | `Object` | Optional | Additional order metadata | Object getMetadata() | setMetadata(Object metadata) |
| `Attributes` | `Map<String, String>` | Optional | - | Map<String, String> getAttributes() | setAttributes(Map<String, String> attributes) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "customerId": "cust_12345",
  "items": [
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
  ],
  "callbackUrl": "https://merchant.example.com/callbacks/payment",
  "attributes": {
    "color": "red",
    "size": "XL"
  },
  "document": "data:text/plain;name=dummy_file;base64,",
  "metadata": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

