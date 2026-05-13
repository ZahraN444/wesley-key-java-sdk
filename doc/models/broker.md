
# Broker

Container for broker details.

## Structure

`Broker`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `BrokerID` | `Integer` | Optional | Export broker who will handle the shipment.<br><br>**Default**: `0` | Integer getBrokerID() | setBrokerID(Integer brokerID) |

## Example (as XML)

```xml
<wtg:Broker xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:BrokerID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:BrokerID>
</wtg:Broker>
```

