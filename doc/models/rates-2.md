
# Rates 2

Container for rates returned for the shipment packages.

## Structure

`Rates2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Rate` | [`List<Rate2>`](../../doc/models/rate-2.md) | Optional | Container for individual rates associated with the package. | List<Rate2> getRate() | setRate(List<Rate2> rate) |

## Example (as XML)

```xml
<wtg:Rates xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Rate xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Rate>
  <wtg:Rate xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Rate>
</wtg:Rates>
```

