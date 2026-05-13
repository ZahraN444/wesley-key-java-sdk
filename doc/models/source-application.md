
# Source Application

Container for app specific source identification elements.

## Structure

`SourceApplication`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ApplicationName` | `String` | Optional | The named instance of the app used to create the transaction. | String getApplicationName() | setApplicationName(String applicationName) |
| `ApplicationBaseName` | `String` | Optional | The base name of the app used to create the transaction. | String getApplicationBaseName() | setApplicationBaseName(String applicationBaseName) |
| `ApplicationVersion` | `String` | Optional | The submitting apps version number. | String getApplicationVersion() | setApplicationVersion(String applicationVersion) |

## Example (as XML)

```xml
<wtg:SourceApplication xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:ApplicationName xmlns:wtg="https://www.wisetechglobal.com/">ApplicationName4</wtg:ApplicationName>
  <wtg:ApplicationBaseName xmlns:wtg="https://www.wisetechglobal.com/">ApplicationBaseName8</wtg:ApplicationBaseName>
  <wtg:ApplicationVersion xmlns:wtg="https://www.wisetechglobal.com/">ApplicationVersion2</wtg:ApplicationVersion>
</wtg:SourceApplication>
```

