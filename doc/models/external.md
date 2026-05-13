
# External

Container for the timings associated with external systems.

## Structure

`External`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `StartTime` | `String` | Required | The time the transaction started to be processed by an external system. | String getStartTime() | setStartTime(String startTime) |
| `EndTime` | `String` | Required | The time the transaction finished processing by an external system. | String getEndTime() | setEndTime(String endTime) |
| `Duration` | `double` | Required | The difference in milliseconds between the processing external start and end times. | double getDuration() | setDuration(double duration) |

## Example (as XML)

```xml
<wtg:External xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:StartTime xmlns:wtg="https://www.wisetechglobal.com/">StartTime6</wtg:StartTime>
  <wtg:EndTime xmlns:wtg="https://www.wisetechglobal.com/">EndTime2</wtg:EndTime>
  <wtg:Duration xmlns:wtg="https://www.wisetechglobal.com/">13.16</wtg:Duration>
</wtg:External>
```

