
# Other Rate Types

Container for the additional rate types to be requested by the transaction.

## Structure

`OtherRateTypes`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RateTypeID` | `List<Integer>` | Optional | Identifier of any other rate required in the response. | List<Integer> getRateTypeID() | setRateTypeID(List<Integer> rateTypeID) |

## Example (as XML)

```xml
<wtg:OtherRateTypes xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:RateTypeID xmlns:wtg="https://www.wisetechglobal.com/">38</wtg:RateTypeID>
  <wtg:RateTypeID xmlns:wtg="https://www.wisetechglobal.com/">37</wtg:RateTypeID>
</wtg:OtherRateTypes>
```

