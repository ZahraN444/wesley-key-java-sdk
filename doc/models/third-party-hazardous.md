
# Third Party Hazardous

Container for details for processing by an external hazardous compliance system.

## Structure

`ThirdPartyHazardous`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `InUse` | `boolean` | Required | Indicates if the shipment was created using a third party hazardous package.<br><br>**Default**: `false` | boolean getInUse() | setInUse(boolean inUse) |
| `CarrierID` | `int` | Required | Numeric identifier for the carrier.<br><br>**Default**: `0` | int getCarrierID() | setCarrierID(int carrierID) |

## Example (as XML)

```xml
<wtg:ThirdPartyHazardous xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:InUse xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:InUse>
  <wtg:CarrierID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:CarrierID>
</wtg:ThirdPartyHazardous>
```

