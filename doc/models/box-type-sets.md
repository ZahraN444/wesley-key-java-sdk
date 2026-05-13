
# Box Type Sets

predefined box types to be used, separated by commas. Will be overridden by boxTypes.

## Structure

`BoxTypeSets`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `BoxTypeSet` | `String` | Optional | Box type set. Acceptable values (as of November 2019) are: "fedex"–FedEx OneRate;"usps"–USPS Priority Flat Rate;“pallet"–full-, half-, and quarter-sized 48"x40” pallets. | String getBoxTypeSet() | setBoxTypeSet(String boxTypeSet) |

## Example (as XML)

```xml
<wtg:BoxTypeSets xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:BoxTypeSet xmlns:wtg="https://www.wisetechglobal.com/">BoxTypeSet4</wtg:BoxTypeSet>
</wtg:BoxTypeSets>
```

