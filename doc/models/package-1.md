
# Package 1

Container for an individual package associated with the transaction.

## Structure

`Package1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Status` | [`Status`](../../doc/models/status.md) | Required | Container for transaction errors and warning elements. | Status getStatus() | setStatus(Status status) |
| `RecordIdentifiers` | [`RecordIdentifiers`](../../doc/models/record-identifiers.md) | Optional | Outer container for transaction identifiers. | RecordIdentifiers getRecordIdentifiers() | setRecordIdentifiers(RecordIdentifiers recordIdentifiers) |
| `AdditionalHandling` | `Boolean` | Optional | Indicates that extra handling measures are required when loading the package.<br><br>**Default**: `false` | Boolean getAdditionalHandling() | setAdditionalHandling(Boolean additionalHandling) |
| `Oversize` | `Integer` | Optional | Indicates if the item is over standard size dimensions.<br><br>**Default**: `0` | Integer getOversize() | setOversize(Integer oversize) |
| `PackageType` | `Integer` | Optional | Numeric identifier for the carrier package type.<br><br>**Default**: `0` | Integer getPackageType() | setPackageType(Integer packageType) |
| `FreightClass` | `String` | Optional | The freight class of the package's content. | String getFreightClass() | setFreightClass(String freightClass) |
| `Currency` | `String` | Optional | The currency code associated with the transaction. | String getCurrency() | setCurrency(String currency) |
| `Weight` | `Double` | Optional | The weight of the package.<br><br>**Default**: `0d` | Double getWeight() | setWeight(Double weight) |
| `ISOCurrencyId` | `Integer` | Optional | The ID of the ISO Currency code in use.<br><br>**Default**: `0` | Integer getISOCurrencyId() | setISOCurrencyId(Integer iSOCurrencyId) |
| `ShipperReference` | `String` | Optional | Primary shipping reference number. | String getShipperReference() | setShipperReference(String shipperReference) |
| `PackageReference` | `String` | Optional | Package reference number. | String getPackageReference() | setPackageReference(String packageReference) |
| `PackageID` | `Integer` | Optional | Unique identifier for the package.<br><br>**Default**: `0` | Integer getPackageID() | setPackageID(Integer packageID) |
| `Shipping` | [`Shipping`](../../doc/models/shipping.md) | Optional | Container for shipping associated with the transaction. | Shipping getShipping() | setShipping(Shipping shipping) |
| `Customer` | [`Customer`](../../doc/models/customer.md) | Optional | Container for customer details. | Customer getCustomer() | setCustomer(Customer customer) |
| `International` | [`International2`](../../doc/models/international-2.md) | Optional | Container for international details associated with the shipment. | International2 getInternational() | setInternational(International2 international) |
| `Rates` | [`Rates1`](../../doc/models/rates-1.md) | Optional | Container all rates associated with the transaction. | Rates1 getRates() | setRates(Rates1 rates) |

## Example (as XML)

```xml
<wtg:Package xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Status xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Status>
  <wtg:AdditionalHandling xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:AdditionalHandling>
  <wtg:Oversize xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Oversize>
  <wtg:PackageType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageType>
  <wtg:Weight xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Weight>
  <wtg:ISOCurrencyId xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:ISOCurrencyId>
  <wtg:PackageID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PackageID>
  <wtg:RecordIdentifiers xmlns:wtg="https://www.wisetechglobal.com/"></wtg:RecordIdentifiers>
  <wtg:FreightClass xmlns:wtg="https://www.wisetechglobal.com/">FreightClass0</wtg:FreightClass>
</wtg:Package>
```

