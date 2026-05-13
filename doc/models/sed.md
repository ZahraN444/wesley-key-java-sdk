
# SED

Container for SED details.

## Structure

`SED`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Method` | `Integer` | Optional | Method to be used to submit Shipper's Export Declaration information for this shipment.<br><br>**Default**: `0` | Integer getMethod() | setMethod(Integer method) |
| `ExemptNumber` | `String` | Optional | Details why the shipment does not require a Shipper's Export Declaration. | String getExemptNumber() | setExemptNumber(String exemptNumber) |

## Example (as XML)

```xml
<wtg:SED xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Method xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Method>
  <wtg:ExemptNumber xmlns:wtg="https://www.wisetechglobal.com/">ExemptNumber8</wtg:ExemptNumber>
</wtg:SED>
```

