
# Package 6

Container for an individual package associated with the transaction.

## Structure

`Package6`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Status` | [`Status`](../../doc/models/status.md) | Required | Container for transaction errors and warning elements. | Status getStatus() | setStatus(Status status) |
| `AdditionalHandling` | `Boolean` | Optional | Indicates that extra handling measures are required when loading the package.<br><br>**Default**: `false` | Boolean getAdditionalHandling() | setAdditionalHandling(Boolean additionalHandling) |
| `Oversize` | `Integer` | Optional | Indicates if the item is over standard size dimensions.<br><br>**Default**: `0` | Integer getOversize() | setOversize(Integer oversize) |
| `PackageType` | `Integer` | Optional | Numeric identifier for the carrier package type.<br><br>**Default**: `0` | Integer getPackageType() | setPackageType(Integer packageType) |
| `FreightClass` | `String` | Optional | The freight class of the package's content. | String getFreightClass() | setFreightClass(String freightClass) |
| `ShipperReference` | `String` | Optional | Primary shipping reference number. | String getShipperReference() | setShipperReference(String shipperReference) |
| `PackageReference` | `String` | Optional | Package reference number, which will be echoed back in the response. | String getPackageReference() | setPackageReference(String packageReference) |
| `International` | [`International7`](../../doc/models/international-7.md) | Optional | Container for international details associated with the shipment. | International7 getInternational() | setInternational(International7 international) |

## Example (as XML)

```xml
<wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Status>
  <wtg:AdditionalHandling xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AdditionalHandling>
  <wtg:Oversize xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Oversize>
  <wtg:PackageType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageType>
  <wtg:FreightClass xmlns:wtg="https://www.wisetechglobal.com/">FreightClass4</wtg:FreightClass>
  <wtg:ShipperReference xmlns:wtg="https://www.wisetechglobal.com/">ShipperReference6</wtg:ShipperReference>
</wtg:Package>
```

