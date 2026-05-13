
# Home Delivery 1

Container for home delivery details.

## Structure

`HomeDelivery1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | `Integer` | Optional | Type of home delivery required for the shipment.<br><br>**Constraints**: *Pattern*: `[1-3]` | Integer getType() | setType(Integer type) |

## Example (as XML)

```xml
<wtg:HomeDelivery xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Type xmlns:wtg="https://www.wisetechglobal.com/">252</wtg:Type>
</wtg:HomeDelivery>
```

