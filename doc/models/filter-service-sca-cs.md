
# Filter Service SCA Cs

Container element carrier service SCAC codes used to filter the results.

## Structure

`FilterServiceSCACs`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FilterServiceSCAC` | `List<String>` | Optional | Used to filter the returned rates to only those with the specified carrier service SCAC.  Only used when Filter Mode = 4. | List<String> getFilterServiceSCAC() | setFilterServiceSCAC(List<String> filterServiceSCAC) |

## Example (as XML)

```xml
<wtg:FilterServiceSCACs xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:FilterServiceSCAC xmlns:wtg="https://www.wisetechglobal.com/">FilterServiceSCAC3</wtg:FilterServiceSCAC>
  <wtg:FilterServiceSCAC xmlns:wtg="https://www.wisetechglobal.com/">FilterServiceSCAC4</wtg:FilterServiceSCAC>
</wtg:FilterServiceSCACs>
```

