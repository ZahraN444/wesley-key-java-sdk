
# Filter SCA Cs

Container element carrier SCAC codes used to filter the results.

## Structure

`FilterSCACs`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FilterSCAC` | `List<String>` | Optional | Used to filter the returned rates to only those with the specified carrier SCAC.  Only used when Filter Mode = 3. | List<String> getFilterSCAC() | setFilterSCAC(List<String> filterSCAC) |

## Example (as XML)

```xml
<wtg:FilterSCACs xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:FilterSCAC xmlns:wtg="https://www.wisetechglobal.com/">FilterSCAC0</wtg:FilterSCAC>
  <wtg:FilterSCAC xmlns:wtg="https://www.wisetechglobal.com/">FilterSCAC1</wtg:FilterSCAC>
</wtg:FilterSCACs>
```

