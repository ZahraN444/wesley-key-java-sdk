
# Order Created Event

*This model accepts additional fields of type Object.*

## Structure

`OrderCreatedEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `OrderId` | `String` | Required | - | String getOrderId() | setOrderId(String orderId) |
| `FulfillmentStatus` | [`FulfillmentStatus`](../../doc/models/fulfillment-status.md) | Required | - | FulfillmentStatus getFulfillmentStatus() | setFulfillmentStatus(FulfillmentStatus fulfillmentStatus) |
| `TrackingNumber` | `String` | Optional | - | String getTrackingNumber() | setTrackingNumber(String trackingNumber) |
| `Carrier` | `String` | Optional | - | String getCarrier() | setCarrier(String carrier) |
| `Scopes` | [`List<OauthScopeOauthACG>`](../../doc/models/oauth-scope-oauth-acg.md) | Optional | List of scopes that apply to the OAuth token<br><br>**Constraints**: *Unique Items Required* | List<OauthScopeOauthACG> getScopes() | setScopes(List<OauthScopeOauthACG> scopes) |
| `EstimatedDelivery` | `LocalDate` | Optional | - | LocalDate getEstimatedDelivery() | setEstimatedDelivery(LocalDate estimatedDelivery) |
| `Timestamp` | `LocalDateTime` | Optional | - | LocalDateTime getTimestamp() | setTimestamp(LocalDateTime timestamp) |
| `Document` | `InputStream` | Optional | Binary file upload | InputStream getDocument() | setDocument(InputStream document) |
| `TotalWeight` | `Double` | Optional | - | Double getTotalWeight() | setTotalWeight(Double totalWeight) |
| `Price` | `Double` | Optional | - | Double getPrice() | setPrice(Double price) |
| `Quantity` | `Integer` | Optional | - | Integer getQuantity() | setQuantity(Integer quantity) |
| `LongId` | `Long` | Optional | - | Long getLongId() | setLongId(Long longId) |
| `Fragile` | `Boolean` | Optional | - | Boolean getFragile() | setFragile(Boolean fragile) |
| `Notes` | `String` | Optional | Explicitly nullable field | String getNotes() | setNotes(String notes) |
| `Items` | `List<String>` | Optional | - | List<String> getItems() | setItems(List<String> items) |
| `Packages` | [`List<Package>`](../../doc/models/package.md) | Optional | - | List<Package> getPackages() | setPackages(List<Package> packages) |
| `Address` | [`Address`](../../doc/models/address.md) | Optional | - | Address getAddress() | setAddress(Address address) |
| `Metadata` | `Object` | Optional | - | Object getMetadata() | setMetadata(Object metadata) |
| `Attributes` | `Map<String, String>` | Optional | - | Map<String, String> getAttributes() | setAttributes(Map<String, String> attributes) |
| `DeliveryDetails` | [`OrderCreatedEventDeliveryDetails`](../../doc/models/containers/order-created-event-delivery-details.md) | Optional | This is a container for one-of cases. | OrderCreatedEventDeliveryDetails getDeliveryDetails() | setDeliveryDetails(OrderCreatedEventDeliveryDetails deliveryDetails) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "orderId": null,
  "fulfillmentStatus": "fulfilled",
  "carrier": "FedEx",
  "estimatedDelivery": "2025-09-22",
  "timestamp": "09/19/2025 14:00:00",
  "totalWeight": 12.75,
  "price": 199.99,
  "quantity": 5,
  "longId": 9223372036854775807,
  "fragile": true,
  "items": [
    "item1",
    "item2"
  ],
  "packages": [
    {
      "packageId": "PKG123",
      "weight": 2.5
    }
  ],
  "address": {
    "street": "123 Main St",
    "city": "New York",
    "zip": "10001"
  },
  "metadata": {
    "customField1": "value",
    "customField2": 123
  },
  "attributes": {
    "color": "red",
    "size": "XL"
  },
  "deliveryDetails": {
    "method": "express",
    "eta": "2025-09-21T12:00:00Z"
  },
  "trackingNumber": "trackingNumber2",
  "scopes": [
    "file_requests.read"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

