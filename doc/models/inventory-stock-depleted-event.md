
# Inventory Stock Depleted Event

*This model accepts additional fields of type Object.*

## Structure

`InventoryStockDepletedEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `InventoryStockDepletedEventType` | `String` | Required, Constant | **Value**: `"stock.depleted"` | String getInventoryStockDepletedEventType() | setInventoryStockDepletedEventType(String inventoryStockDepletedEventType) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "inventoryStockDepletedEventType": "stock.depleted",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

