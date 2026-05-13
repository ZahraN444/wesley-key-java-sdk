
# Quote

Container for quote information.

## Structure

`Quote`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `QuoteID` | `String` | Optional | Identifier of the rate quote selected for the shipment.<br><br>**Default**: `"0"` | String getQuoteID() | setQuoteID(String quoteID) |
| `OptionID` | `String` | Optional | Identifier of the rate option selected for the shipment.<br><br>**Default**: `"0"` | String getOptionID() | setOptionID(String optionID) |
| `SCAC` | `String` | Optional | Identifier of the rate scac selected for the shipment. | String getSCAC() | setSCAC(String sCAC) |

## Example (as XML)

```xml
<wtg:Quote xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:QuoteID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:QuoteID>
  <wtg:OptionID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:OptionID>
  <wtg:SCAC xmlns:wtg="https://www.wisetechglobal.com/">SCAC4</wtg:SCAC>
</wtg:Quote>
```

