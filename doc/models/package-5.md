
# Package 5

Container for an individual package associated with the transaction.

## Structure

`Package5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Weight` | `Double` | Optional | The weight of the package.<br><br>**Default**: `0d` | Double getWeight() | setWeight(Double weight) |
| `Length` | `Double` | Optional | The dimensional lenth of the package.<br><br>**Default**: `0d` | Double getLength() | setLength(Double length) |
| `Width` | `Double` | Optional | The dimensional width of the package.<br><br>**Default**: `0d` | Double getWidth() | setWidth(Double width) |
| `Height` | `Double` | Optional | The dimensional height of the package.<br><br>**Default**: `0d` | Double getHeight() | setHeight(Double height) |
| `FreightClass` | `String` | Optional | The freight class of the package's content. | String getFreightClass() | setFreightClass(String freightClass) |
| `NMFC` | `String` | Optional | The National Motor Freight Classification of the package. | String getNMFC() | setNMFC(String nMFC) |
| `PalletCount` | `Integer` | Optional | Number of pallets.<br><br>**Default**: `0` | Integer getPalletCount() | setPalletCount(Integer palletCount) |
| `ItemsOnPallet` | `Integer` | Optional | Number of items on the pallet.<br><br>**Default**: `0` | Integer getItemsOnPallet() | setItemsOnPallet(Integer itemsOnPallet) |
| `International` | [`International6`](../../doc/models/international-6.md) | Optional | Container for international details associated with the shipment. | International6 getInternational() | setInternational(International6 international) |

## Example (as XML)

```xml
<wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Weight>
  <wtg:Length xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Length>
  <wtg:Width xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Width>
  <wtg:Height xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Height>
  <wtg:PalletCount xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PalletCount>
  <wtg:ItemsOnPallet xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ItemsOnPallet>
  <wtg:FreightClass xmlns:wtg="https://www.wisetechglobal.com/">FreightClass4</wtg:FreightClass>
</wtg:Package>
```

