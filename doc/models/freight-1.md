
# Freight 1

Container for freight specific values

## Structure

`Freight1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Billing` | [`Billing1`](../../doc/models/billing-1.md) | Optional | Container for billing details associated with the transaction. | Billing1 getBilling() | setBilling(Billing1 billing) |
| `FreightHandlingLength` | `Double` | Optional | The dimensional length of the freight handling type. Only to be used when rate shopping with a rategroup that contains both LTL and Parcel services.<br><br>**Default**: `0d` | Double getFreightHandlingLength() | setFreightHandlingLength(Double freightHandlingLength) |
| `FreightHandlingWidth` | `Double` | Optional | The dimensional width of the freight handling type. Only to be used when rate shopping with a rategroup that contains both LTL and Parcel services.<br><br>**Default**: `0d` | Double getFreightHandlingWidth() | setFreightHandlingWidth(Double freightHandlingWidth) |
| `FreightHandlingHeight` | `Double` | Optional | The dimensional height of the freight handling type. Only to be used when rate shopping with a rategroup that contains both LTL and Parcel services.<br><br>**Default**: `0d` | Double getFreightHandlingHeight() | setFreightHandlingHeight(Double freightHandlingHeight) |
| `FreightHandlingPalletWeight` | `Double` | Optional | The weight of the pallet. Only to be used when rate shopping with a rategroup that contains both LTL and Parcel services.<br><br>**Default**: `0d` | Double getFreightHandlingPalletWeight() | setFreightHandlingPalletWeight(Double freightHandlingPalletWeight) |
| `MixedFreightParcelMode` | `Boolean` | Optional | Indicates if the rateshop has a mixture of parcel and freight carriers<br><br>**Default**: `false` | Boolean getMixedFreightParcelMode() | setMixedFreightParcelMode(Boolean mixedFreightParcelMode) |
| `FreightClass` | `String` | Optional | The freight class of the package's content. | String getFreightClass() | setFreightClass(String freightClass) |
| `NMFC` | `String` | Optional | The National Motor Freight Classification of the package. | String getNMFC() | setNMFC(String nMFC) |
| `ShipAfterTime` | `String` | Optional | ShipAfterTime for a a Freight Shipment | String getShipAfterTime() | setShipAfterTime(String shipAfterTime) |
| `ShipBeforeTime` | `String` | Optional | ShipBeforeTime for a a Freight Shipment | String getShipBeforeTime() | setShipBeforeTime(String shipBeforeTime) |

## Example (as XML)

```xml
<wtg:Freight xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:FreightHandlingLength xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:FreightHandlingLength>
  <wtg:FreightHandlingWidth xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:FreightHandlingWidth>
  <wtg:FreightHandlingHeight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:FreightHandlingHeight>
  <wtg:FreightHandlingPalletWeight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:FreightHandlingPalletWeight>
  <wtg:MixedFreightParcelMode xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:MixedFreightParcelMode>
  <wtg:Billing xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Billing>
</wtg:Freight>
```

