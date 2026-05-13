
# Output 1

Container for labels to be printed externally from the transaction.

## Structure

`Output1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Guid` | `String` | Optional | Unique identifier for the printed output can be used to reprint. | String getGuid() | setGuid(String guid) |
| `Type` | `int` | Required | A numeric identifier that identifies the type of label. | int getType() | setType(int type) |
| `Description` | `String` | Optional | Description of the output that has been produced, e.g. Label. | String getDescription() | setDescription(String description) |
| `Format` | `Integer` | Optional | A numeric identifier that identifies the format of the label. | Integer getFormat() | setFormat(Integer format) |
| `MimeType` | `String` | Optional | If appropriate the internet media type associated with the label format. | String getMimeType() | setMimeType(String mimeType) |
| `HubCappServerUri` | `String` | Optional | If appropriate the configured HubCapp Server address. | String getHubCappServerUri() | setHubCappServerUri(String hubCappServerUri) |
| `HubCappLicenseKey` | `String` | Optional | If appropriate the License Key associated with the HubCapp instance. | String getHubCappLicenseKey() | setHubCappLicenseKey(String hubCappLicenseKey) |
| `HubCappMachineID` | `String` | Optional | If appropriate HubCapp communications channel name. | String getHubCappMachineID() | setHubCappMachineID(String hubCappMachineID) |
| `Content` | `String` | Optional | If appropriate for the printing type, a base 64 encoded value for the label. | String getContent() | setContent(String content) |
| `Stock` | `Integer` | Optional | A numeric identifier for the stock type of the output.<br><br>**Default**: `0` | Integer getStock() | setStock(Integer stock) |
| `Pages` | [`Pages`](../../doc/models/pages.md) | Optional | Container for all pages to be printed by the caller of the transaction (client). | Pages getPages() | setPages(Pages pages) |
| `Status` | [`Status2`](../../doc/models/status-2.md) | Optional | Container for HubCapp printing status. | Status2 getStatus() | setStatus(Status2 status) |
| `Printed` | `Boolean` | Optional | Indicates the remote HubCapp print completed. | Boolean getPrinted() | setPrinted(Boolean printed) |

## Example (as XML)

```xml
<wtg:Output xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Type xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Type>
  <wtg:Stock xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Stock>
  <wtg:Guid xmlns:wtg="https://www.wisetechglobal.com/">Guid4</wtg:Guid>
  <wtg:Description xmlns:wtg="https://www.wisetechglobal.com/">Description2</wtg:Description>
  <wtg:Format xmlns:wtg="https://www.wisetechglobal.com/">252</wtg:Format>
  <wtg:MimeType xmlns:wtg="https://www.wisetechglobal.com/">MimeType0</wtg:MimeType>
  <wtg:HubCappServerUri xmlns:wtg="https://www.wisetechglobal.com/">HubCappServerUri4</wtg:HubCappServerUri>
</wtg:Output>
```

