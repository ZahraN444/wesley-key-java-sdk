
# Processing

Container element for transaction processing statistics.

## Structure

`Processing`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `StartTime` | `String` | Required | The time the transaction started to be processed. | String getStartTime() | setStartTime(String startTime) |
| `EndTime` | `String` | Required | The time the transaction finished processing. | String getEndTime() | setEndTime(String endTime) |
| `Duration` | `double` | Required | The difference in milliseconds between the processing start and end times. | double getDuration() | setDuration(double duration) |
| `External` | [`External`](../../doc/models/external.md) | Optional | Container for the timings associated with external systems. | External getExternal() | setExternal(External external) |
| `ServerName` | `String` | Required | The Net BIOS name of the server which processed the transaction. | String getServerName() | setServerName(String serverName) |
| `UserName` | `String` | Optional | The authorized name of the user under which the transaction was processed. | String getUserName() | setUserName(String userName) |

## Example (as XML)

```xml
<wtg:Processing xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:StartTime xmlns:wtg="https://www.wisetechglobal.com/">StartTime4</wtg:StartTime>
  <wtg:EndTime xmlns:wtg="https://www.wisetechglobal.com/">EndTime0</wtg:EndTime>
  <wtg:Duration xmlns:wtg="https://www.wisetechglobal.com/">252.24</wtg:Duration>
  <wtg:External xmlns:wtg="https://www.wisetechglobal.com/"></wtg:External>
  <wtg:ServerName xmlns:wtg="https://www.wisetechglobal.com/">ServerName6</wtg:ServerName>
  <wtg:UserName xmlns:wtg="https://www.wisetechglobal.com/">UserName2</wtg:UserName>
</wtg:Processing>
```

