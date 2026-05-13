
# Track Status

Container for tracking history state details.

## Structure

`TrackStatus`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ID` | `Integer` | Optional | Unique numeric identifier for the tracking history record. | Integer getID() | setID(Integer iD) |
| `Description` | `String` | Required | The free form description for the package history state. | String getDescription() | setDescription(String description) |
| `Location` | `String` | Optional | The description of the location that the event occured, if available. | String getLocation() | setLocation(String location) |
| `Date` | `String` | Optional | The date that the event occured, if available. | String getDate() | setDate(String date) |
| `Time` | `String` | Optional | The time that the event occured, if available. | String getTime() | setTime(String time) |
| `SignedForBy` | `String` | Optional | The name of the person that signed for the package on delivery, if available. | String getSignedForBy() | setSignedForBy(String signedForBy) |

## Example (as XML)

```xml
<wtg:TrackStatus xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ID xmlns:wtg="https://www.wisetechglobal.com/">184</wtg:ID>
  <wtg:Description xmlns:wtg="https://www.wisetechglobal.com/">Description0</wtg:Description>
  <wtg:Location xmlns:wtg="https://www.wisetechglobal.com/">Location0</wtg:Location>
  <wtg:Date xmlns:wtg="https://www.wisetechglobal.com/">Date4</wtg:Date>
  <wtg:Time xmlns:wtg="https://www.wisetechglobal.com/">Time8</wtg:Time>
  <wtg:SignedForBy xmlns:wtg="https://www.wisetechglobal.com/">SignedForBy2</wtg:SignedForBy>
</wtg:TrackStatus>
```

