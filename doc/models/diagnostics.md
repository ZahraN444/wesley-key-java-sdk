
# Diagnostics

Container for logging and diagnostic override elements.

## Structure

`Diagnostics`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `LogLevel` | [`LogLevelEnum`](../../doc/models/log-level-enum.md) | Optional | If provided overrides the level of diagnostic logging associated with the transaction.  If omitted the system configured value is used. | LogLevelEnum getLogLevel() | setLogLevel(LogLevelEnum logLevel) |
| `TraceThreshold` | `Double` | Optional | If provided overrides the threshold associated with trace level logging.  If omitted the system configured value is used. | Double getTraceThreshold() | setTraceThreshold(Double traceThreshold) |
| `MaximumRowsToLog` | `Integer` | Optional | If provided overrides the maximum number of rows to log using trace level logging.  If omitted the system configured value is used. | Integer getMaximumRowsToLog() | setMaximumRowsToLog(Integer maximumRowsToLog) |

## Example (as XML)

```xml
<wtg:Diagnostics xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:LogLevel xmlns:wtg="https://www.wisetechglobal.com/">Warn</wtg:LogLevel>
  <wtg:TraceThreshold xmlns:wtg="https://www.wisetechglobal.com/">23.94</wtg:TraceThreshold>
  <wtg:MaximumRowsToLog xmlns:wtg="https://www.wisetechglobal.com/">60</wtg:MaximumRowsToLog>
</wtg:Diagnostics>
```

