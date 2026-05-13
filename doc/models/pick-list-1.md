
# Pick List 1

Container for an individual picklist.

## Structure

`PickList1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PickListID` | `Integer` | Optional | Identifier of the pick list being shipped.<br><br>**Default**: `0` | Integer getPickListID() | setPickListID(Integer pickListID) |
| `PickListNumber` | `String` | Required | Unique number of the pick list being shipped. | String getPickListNumber() | setPickListNumber(String pickListNumber) |

## Example (as XML)

```xml
<wtg:PickList xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:PickListID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PickListID>
  <wtg:PickListNumber xmlns:wtg="https://www.wisetechglobal.com/"></wtg:PickListNumber>
</wtg:PickList>
```

