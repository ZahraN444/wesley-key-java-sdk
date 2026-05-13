
# Pierbridge Track Request

Requests the latest tracking status of a shipment with a carrier.

## Structure

`PierbridgeTrackRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TransactionIdentifier` | `String` | Optional | A unique identifier for the transaction, this value is not used during processing and will be returned in the response. | String getTransactionIdentifier() | setTransactionIdentifier(String transactionIdentifier) |
| `ControlIdentifier` | `String` | Optional | A reference to a control which generated the request, this value is not used during processing and will be returned in the response. | String getControlIdentifier() | setControlIdentifier(String controlIdentifier) |
| `UserName` | `String` | Required | The user name to use when processing the transaction.<br><br>**Constraints**: *Minimum Length*: `1` | String getUserName() | setUserName(String userName) |
| `Live` | `Boolean` | Optional | Indicates whether the transaction is a test or live.  Defaults to system configured value if not submitted.<br><br>**Default**: `false` | Boolean getLive() | setLive(Boolean live) |
| `Carrier` | `Integer` | Optional | Numeric identifier for the carrier.<br><br>**Default**: `0` | Integer getCarrier() | setCarrier(Integer carrier) |
| `BoLNumber` | `String` | Optional | BoL Number of the shipment to track. | String getBoLNumber() | setBoLNumber(String boLNumber) |
| `Sender` | [`Sender3`](../../doc/models/sender-3.md) | Optional | Container to allow the tracking by Sender DepartmentName. | Sender3 getSender() | setSender(Sender3 sender) |
| `Packages` | [`Packages10`](../../doc/models/packages-10.md) | Required | Container for all packages associated with the transaction. | Packages10 getPackages() | setPackages(Packages10 packages) |
| `Diagnostics` | [`Diagnostics`](../../doc/models/diagnostics.md) | Optional | Container for logging and diagnostic override elements. | Diagnostics getDiagnostics() | setDiagnostics(Diagnostics diagnostics) |
| `Identification` | [`Identification`](../../doc/models/identification.md) | Optional | Container for client identification elements. | Identification getIdentification() | setIdentification(Identification identification) |

## Example (as XML)

```xml
<wtg:PierbridgeTrackRequest xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:UserName xmlns:wtg="https://www.wisetechglobal.com/"></wtg:UserName>
  <wtg:Live xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Live>
  <wtg:Carrier xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Carrier>
  <wtg:Packages xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:Package>
      <wtg:AccountID>0</wtg:AccountID>
      <wtg:PackageID>0</wtg:PackageID>
      <wtg:WayBillNumber>WayBillNumber6</wtg:WayBillNumber>
      <wtg:ShipperReference>ShipperReference8</wtg:ShipperReference>
      <wtg:ReferenceOne>ReferenceOne8</wtg:ReferenceOne>
    </wtg:Package>
  </wtg:Packages>
  <wtg:TransactionIdentifier xmlns:wtg="https://www.wisetechglobal.com/">TransactionIdentifier0</wtg:TransactionIdentifier>
  <wtg:ControlIdentifier xmlns:wtg="https://www.wisetechglobal.com/">ControlIdentifier0</wtg:ControlIdentifier>
  <wtg:BoLNumber xmlns:wtg="https://www.wisetechglobal.com/">BoLNumber4</wtg:BoLNumber>
</wtg:PierbridgeTrackRequest>
```

