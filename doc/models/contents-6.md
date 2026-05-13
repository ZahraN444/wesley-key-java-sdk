
# Contents 6

Container for all contents (line items) associated with the transaction.

## Structure

`Contents6`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Content` | [`List<Content6>`](../../doc/models/content-6.md) | Required | Container for a individual content (line item) associated with the transaction. | List<Content6> getContent() | setContent(List<Content6> content) |

## Example (as XML)

```xml
<wtg:Contents xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Content xmlns:wtg="https://www.wisetechglobal.com/">
    <wtg:Quantity>0</wtg:Quantity>
    <wtg:OrderedQuantity>0</wtg:OrderedQuantity>
    <wtg:BackOrderedQuantity>0</wtg:BackOrderedQuantity>
    <wtg:ContentLineValue>0</wtg:ContentLineValue>
    <wtg:Value>0</wtg:Value>
    <wtg:Weight>0</wtg:Weight>
    <wtg:TotalWeight>0</wtg:TotalWeight>
    <wtg:Hazardous>false</wtg:Hazardous>
    <wtg:HazardousExemptionID>0</wtg:HazardousExemptionID>
    <wtg:HazardousUnits>0</wtg:HazardousUnits>
    <wtg:HazardousTotalQuantity>0</wtg:HazardousTotalQuantity>
    <wtg:HazardousLabelCodesMask>0</wtg:HazardousLabelCodesMask>
    <wtg:HazardousAccessible>false</wtg:HazardousAccessible>
    <wtg:HazardousPassengerAircraft>false</wtg:HazardousPassengerAircraft>
    <wtg:HazardousCargoAircraftOnly>false</wtg:HazardousCargoAircraftOnly>
    <wtg:HazardousConsumerCommodity>false</wtg:HazardousConsumerCommodity>
    <wtg:HazardousLimitedQuantity>false</wtg:HazardousLimitedQuantity>
    <wtg:HazardousConcentration>0</wtg:HazardousConcentration>
    <wtg:Hazardous500KGExemption>false</wtg:Hazardous500KGExemption>
    <wtg:HazardousOverpack>false</wtg:HazardousOverpack>
    <wtg:HazardousAllInOne>false</wtg:HazardousAllInOne>
    <wtg:SenderIsProducer>false</wtg:SenderIsProducer>
    <wtg:JointProduction>false</wtg:JointProduction>
    <wtg:ProducerEvidence>0</wtg:ProducerEvidence>
    <wtg:RegionalValueContentCalculatedUsingNetCostMethod>false</wtg:RegionalValueContentCalculatedUsingNetCostMethod>
    <wtg:HazardousSQEIndicator>false</wtg:HazardousSQEIndicator>
    <wtg:NetMassQuantity>0</wtg:NetMassQuantity>
    <wtg:RecordIdentifiers></wtg:RecordIdentifiers>
    <wtg:Radionuclide></wtg:Radionuclide>
    <wtg:Code>Code6</wtg:Code>
  </wtg:Content>
</wtg:Contents>
```

