
# Output 3

Container for documents to be printed externally from the transaction.

## Structure

`Output3`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Guid` | `String` | Optional | Unique identifier for the printed output can be used to reprint. | String getGuid() | setGuid(String guid) |
| `Type` | `int` | Required | A numeric identifier that identifies the type of document. | int getType() | setType(int type) |
| `Description` | `String` | Optional | Description of the output that has been produced, e.g. Report. | String getDescription() | setDescription(String description) |
| `Format` | `int` | Required | A numeric identifier that identifies the format of the document. | int getFormat() | setFormat(int format) |
| `MimeType` | `String` | Optional | If appropriate the internet media type associated with the document format. | String getMimeType() | setMimeType(String mimeType) |
| `HubCappServerUri` | `String` | Optional | If appropriate the configured HubCapp Server address. | String getHubCappServerUri() | setHubCappServerUri(String hubCappServerUri) |
| `HubCappLicenseKey` | `String` | Optional | If appropriate the License Key associated with the HubCapp instance. | String getHubCappLicenseKey() | setHubCappLicenseKey(String hubCappLicenseKey) |
| `HubCappMachineID` | `String` | Optional | If appropriate HubCapp communications channel name. | String getHubCappMachineID() | setHubCappMachineID(String hubCappMachineID) |
| `Content` | `String` | Optional | If appropriate for the printing type, a base 64 encoded value for the document. | String getContent() | setContent(String content) |
| `Stock` | `Integer` | Optional | A numeric identifier for the stock type of the output.<br><br>**Default**: `0` | Integer getStock() | setStock(Integer stock) |
| `Pages` | [`Pages`](../../doc/models/pages.md) | Optional | Container for all pages to be printed by the caller of the transaction (client). | Pages getPages() | setPages(Pages pages) |
| `Status` | [`Status2`](../../doc/models/status-2.md) | Optional | Container for HubCapp printing status. | Status2 getStatus() | setStatus(Status2 status) |
| `Printed` | `Boolean` | Optional | Indicates the remote HubCapp print completed. | Boolean getPrinted() | setPrinted(Boolean printed) |

## Example (as XML)

```xml
<wtg:Output xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:Type xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Type>
  <wtg:Format xmlns:wtg="https://www.wisetechglobal.com/"></wtg:Format>
  <wtg:Stock xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Stock>
  <wtg:Guid xmlns:wtg="https://www.wisetechglobal.com/">Guid8</wtg:Guid>
  <wtg:Description xmlns:wtg="https://www.wisetechglobal.com/">Description0</wtg:Description>
  <wtg:MimeType xmlns:wtg="https://www.wisetechglobal.com/">MimeType2</wtg:MimeType>
  <wtg:HubCappServerUri xmlns:wtg="https://www.wisetechglobal.com/">HubCappServerUri6</wtg:HubCappServerUri>
  <wtg:HubCappLicenseKey xmlns:wtg="https://www.wisetechglobal.com/">HubCappLicenseKey4</wtg:HubCappLicenseKey>
</wtg:Output>
```

