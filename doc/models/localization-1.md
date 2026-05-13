
# Localization 1

Container for localization information.

## Structure

`Localization1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TimeZoneCode` | `String` | Required | Code of the timezone that the executing user is in.<br><br>**Default**: `"0"` | String getTimeZoneCode() | setTimeZoneCode(String timeZoneCode) |
| `TimeZoneName` | `String` | Required | Name of the timezone that the executing user is in.<br><br>**Default**: `"0"` | String getTimeZoneName() | setTimeZoneName(String timeZoneName) |
| `TimeZoneOffset` | `String` | Required | Name of the timezone that the executing user is in.<br><br>**Default**: `"0"` | String getTimeZoneOffset() | setTimeZoneOffset(String timeZoneOffset) |

## Example (as XML)

```xml
<wtg:Localization xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:TimeZoneCode xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TimeZoneCode>
  <wtg:TimeZoneName xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TimeZoneName>
  <wtg:TimeZoneOffset xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:TimeZoneOffset>
</wtg:Localization>
```

