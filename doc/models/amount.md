
# Amount

Container for net explosive amount details.

## Structure

`Amount`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Quantity` | `Double` | Optional | Net explosive quantity. | Double getQuantity() | setQuantity(Double quantity) |
| `UOM` | `String` | Optional | Net explosive units of measure. | String getUOM() | setUOM(String uOM) |

## Example (as XML)

```xml
<wtg:Amount xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Quantity xmlns:wtg="https://www.wisetechglobal.com/">203.34</wtg:Quantity>
  <wtg:UOM xmlns:wtg="https://www.wisetechglobal.com/">UOM6</wtg:UOM>
</wtg:Amount>
```

