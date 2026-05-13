
# Package 4

Container for package level information about the rate returned.

## Structure

`Package4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Rates` | [`Rates2`](../../doc/models/rates-2.md) | Required | Container for rates returned for the shipment packages. | Rates2 getRates() | setRates(Rates2 rates) |

## Example (as XML)

```xml
<wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Rates xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Rates>
</wtg:Package>
```

