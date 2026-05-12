
# Inventory Change Event Body

## Class Name

`InventoryChangeEventBody`

## Cases

| Type | Factory Method |
|  --- | --- |
| [`InventoryStockIncreaseEvent`](../../../doc/models/inventory-stock-increase-event.md) | InventoryChangeEventBody.fromInventoryStockIncreaseEvent(InventoryStockIncreaseEvent inventoryStockIncreaseEvent) |
| [`InventoryStockDecreaseEvent`](../../../doc/models/inventory-stock-decrease-event.md) | InventoryChangeEventBody.fromInventoryStockDecreaseEvent(InventoryStockDecreaseEvent inventoryStockDecreaseEvent) |
| [`InventoryStockDepletedEvent`](../../../doc/models/inventory-stock-depleted-event.md) | InventoryChangeEventBody.fromInventoryStockDepletedEvent(InventoryStockDepletedEvent inventoryStockDepletedEvent) |

## InventoryStockIncreaseEvent

### Initialization Code

#### Example

```java
InventoryChangeEventBody.fromInventoryStockIncreaseEvent(
        new InventoryStockIncreaseEvent.Builder(
            "stock.increase"
        )
        .build()
    )
```

## InventoryStockDecreaseEvent

### Initialization Code

#### Example

```java
InventoryChangeEventBody.fromInventoryStockDecreaseEvent(
        new InventoryStockDecreaseEvent.Builder(
            "stock.decrease"
        )
        .build()
    )
```

## InventoryStockDepletedEvent

### Initialization Code

#### Example

```java
InventoryChangeEventBody.fromInventoryStockDepletedEvent(
        new InventoryStockDepletedEvent.Builder(
            "stock.depleted"
        )
        .build()
    )
```

