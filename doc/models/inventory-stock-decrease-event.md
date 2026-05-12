
# Inventory Stock Decrease Event

*This model accepts additional fields of type Object.*

## Structure

`InventoryStockDecreaseEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `InventoryStockDecreaseEventType` | `String` | Required, Constant | **Value**: `"stock.decrease"` | String getInventoryStockDecreaseEventType() | setInventoryStockDecreaseEventType(String inventoryStockDecreaseEventType) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "inventoryStockDecreaseEventType": "stock.decrease",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

