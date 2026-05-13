
# Net Explosive

Container for net explosive details.

## Structure

`NetExplosive`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Amount` | [`Amount`](../../doc/models/amount.md) | Optional | Container for net explosive amount details. | Amount getAmount() | setAmount(Amount amount) |
| `Abbreviation` | [`AbbreviationEnum`](../../doc/models/abbreviation-enum.md) | Optional | Net explosive abbreviation | AbbreviationEnum getAbbreviation() | setAbbreviation(AbbreviationEnum abbreviation) |

## Example (as XML)

```xml
<wtg:NetExplosive xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Amount xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Amount>
  <wtg:Abbreviation xmlns:wtg="https://www.wisetechglobal.com/">NEW</wtg:Abbreviation>
</wtg:NetExplosive>
```

