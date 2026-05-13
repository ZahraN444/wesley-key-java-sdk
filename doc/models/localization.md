
# Localization

Container for the additional rate types to be requested by the transaction.

## Structure

`Localization`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `WeightUnits` | `String` | Optional | Weight units in use by the current user. | String getWeightUnits() | setWeightUnits(String weightUnits) |
| `DimensionUnits` | `String` | Optional | Dimension units in use by the current user. | String getDimensionUnits() | setDimensionUnits(String dimensionUnits) |
| `CurrencyCode` | `String` | Optional | ISO currency code in use by the current user. | String getCurrencyCode() | setCurrencyCode(String currencyCode) |
| `Culture` | `String` | Optional | Culture code in use by the current user. | String getCulture() | setCulture(String culture) |

## Example (as XML)

```xml
<wtg:Localization xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:WeightUnits xmlns:wtg="https://www.wisetechglobal.com/">WeightUnits4</wtg:WeightUnits>
  <wtg:DimensionUnits xmlns:wtg="https://www.wisetechglobal.com/">DimensionUnits4</wtg:DimensionUnits>
  <wtg:CurrencyCode xmlns:wtg="https://www.wisetechglobal.com/">CurrencyCode6</wtg:CurrencyCode>
  <wtg:Culture xmlns:wtg="https://www.wisetechglobal.com/">Culture0</wtg:Culture>
</wtg:Localization>
```

