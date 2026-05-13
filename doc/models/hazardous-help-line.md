
# Hazardous Help Line

Container for the Hazardous Helpline details associated with the transaction.

## Structure

`HazardousHelpLine`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Phone` | `String` | Optional | Phone number of the Hazardous Helpline. | String getPhone() | setPhone(String phone) |
| `Name` | `String` | Optional | Contact name for the Hazardous Helpline. | String getName() | setName(String name) |
| `ContractNumber` | `String` | Optional | Contract number for the Hazardous Helpline. | String getContractNumber() | setContractNumber(String contractNumber) |

## Example (as XML)

```xml
<wtg:HazardousHelpLine xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Phone xmlns:wtg="https://www.wisetechglobal.com/">Phone2</wtg:Phone>
  <wtg:Name xmlns:wtg="https://www.wisetechglobal.com/">Name4</wtg:Name>
  <wtg:ContractNumber xmlns:wtg="https://www.wisetechglobal.com/">ContractNumber4</wtg:ContractNumber>
</wtg:HazardousHelpLine>
```

