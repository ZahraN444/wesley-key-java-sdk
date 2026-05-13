
# Automated Postage Add

Container for postal meter details.

## Structure

`AutomatedPostageAdd`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TotalSpend` | `String` | Optional | The amount of money remaining on the physical meter. | String getTotalSpend() | setTotalSpend(String totalSpend) |
| `PostageRemaining` | `String` | Optional | The number of records that are remaining in the database that also match the search expression. | String getPostageRemaining() | setPostageRemaining(String postageRemaining) |
| `LowFundsLimit` | `Double` | Optional | The value of the low funds alert.<br><br>**Default**: `0d` | Double getLowFundsLimit() | setLowFundsLimit(Double lowFundsLimit) |
| `LowFundsAlertTypeID` | `Double` | Optional | The low fund alert type identifier.<br><br>**Default**: `0d` | Double getLowFundsAlertTypeID() | setLowFundsAlertTypeID(Double lowFundsAlertTypeID) |
| `SerialNumber` | `Double` | Optional | Serial number for physical meter.<br><br>**Default**: `0d` | Double getSerialNumber() | setSerialNumber(Double serialNumber) |

## Example (as XML)

```xml
<wtg:AutomatedPostageAdd xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:LowFundsLimit xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:LowFundsLimit>
  <wtg:LowFundsAlertTypeID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:LowFundsAlertTypeID>
  <wtg:SerialNumber xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:SerialNumber>
  <wtg:TotalSpend xmlns:wtg="https://www.wisetechglobal.com/">TotalSpend0</wtg:TotalSpend>
  <wtg:PostageRemaining xmlns:wtg="https://www.wisetechglobal.com/">PostageRemaining4</wtg:PostageRemaining>
</wtg:AutomatedPostageAdd>
```

