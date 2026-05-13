
# Output

Container for an output the transaction should generate or customize the printing of.

## Structure

`Output`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `OutputType` | `Integer` | Optional | Type of output.  Defaults to all output types if not submitted.<br><br>**Default**: `0` | Integer getOutputType() | setOutputType(Integer outputType) |
| `UseOutputTypeRule` | `Boolean` | Optional | Indicates whether to use the inbuilt rules to determine if the specified output type should be produced. Only used if output type identifier is specified. Defaults to false if not submitted.<br><br>**Default**: `false` | Boolean getUseOutputTypeRule() | setUseOutputTypeRule(Boolean useOutputTypeRule) |
| `Suppress` | `Boolean` | Optional | Indicates whether to suppress the generation of the output. Defaults to false if not submitted.<br><br>**Default**: `false` | Boolean getSuppress() | setSuppress(Boolean suppress) |
| `Format` | `Integer` | Optional | A numeric identifier that identifies the format of the output.<br><br>**Default**: `0` | Integer getFormat() | setFormat(Integer format) |
| `PrinterDevice` | `Integer` | Optional | Sets the printing method to use for the output (client, windows etc).  Defaults to current configuration if not submitted.<br><br>**Default**: `0` | Integer getPrinterDevice() | setPrinterDevice(Integer printerDevice) |
| `Stock` | `Integer` | Optional | A numeric identifier for the stock type of the output.<br><br>**Default**: `0` | Integer getStock() | setStock(Integer stock) |
| `PrinterModel` | `Integer` | Optional | Sets the PrinterModel to use for the output.  Defaults to current configuration if not submitted.<br><br>**Default**: `0` | Integer getPrinterModel() | setPrinterModel(Integer printerModel) |
| `Copies` | `Integer` | Optional | Number of copies of the specified output.  Defaults to one if not submitted.<br><br>**Default**: `0` | Integer getCopies() | setCopies(Integer copies) |
| `Pieces` | `Integer` | Optional | Number of pieces (e.g. packages, pallets) to produce the output for.  For example, produces labels with ' 1 of 2' and '2 or 2' indicators.  Defaults to one if not submitted.<br><br>**Default**: `0` | Integer getPieces() | setPieces(Integer pieces) |
| `PiecesStartAt` | `Integer` | Optional | Used when chaining together more than one shipment that requires labels with '1 of 2' and '2 or 2' indicators.  Indicators for packages in this shipment will start at this value, e.g. if set to 4 then indicators will start at '4 of ...'.  Defaults to one if not submitted.<br><br>**Default**: `0` | Integer getPiecesStartAt() | setPiecesStartAt(Integer piecesStartAt) |
| `PrintLater` | `Boolean` | Optional | Indicates whether the output should be printed at a later time. Defaults to configured value if not submitted.<br><br>**Default**: `false` | Boolean getPrintLater() | setPrintLater(Boolean printLater) |
| `PrinterID` | `Integer` | Optional | Printer to use when producing the output.  Default printer used if not submitted.<br><br>**Default**: `0` | Integer getPrinterID() | setPrinterID(Integer printerID) |
| `PrintToClient` | `Boolean` | Optional | Forces the return of the output to the client.  Default printing method used if not submitted.<br><br>**Default**: `false` | Boolean getPrintToClient() | setPrintToClient(Boolean printToClient) |

## Example (as XML)

```xml
<wtg:Output xmlns:wtg="https://www.wisetechglobal.com/">
  <wtg:OutputType xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:OutputType>
  <wtg:UseOutputTypeRule xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:UseOutputTypeRule>
  <wtg:Suppress xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:Suppress>
  <wtg:Format xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Format>
  <wtg:PrinterDevice xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PrinterDevice>
  <wtg:Stock xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Stock>
  <wtg:PrinterModel xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PrinterModel>
  <wtg:Copies xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Copies>
  <wtg:Pieces xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:Pieces>
  <wtg:PiecesStartAt xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PiecesStartAt>
  <wtg:PrintLater xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PrintLater>
  <wtg:PrinterID xmlns:wtg="https://www.wisetechglobal.com/">0</wtg:PrinterID>
  <wtg:PrintToClient xmlns:wtg="https://www.wisetechglobal.com/">false</wtg:PrintToClient>
</wtg:Output>
```

