
# Inventory Stock Increase Event

*This model accepts additional fields of type Object.*

## Structure

`InventoryStockIncreaseEvent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `InventoryStockIncreaseEventType` | `String` | Required, Constant | **Value**: `"stock.increase"` | String getInventoryStockIncreaseEventType() | setInventoryStockIncreaseEventType(String inventoryStockIncreaseEventType) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "inventoryStockIncreaseEventType": "stock.increase",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

