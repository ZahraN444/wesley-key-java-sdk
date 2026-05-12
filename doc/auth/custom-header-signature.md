
# Custom Header Signature



Documentation for accessing and setting credentials for ApiKey.

## Auth Credentials

| Name | Type | Description | Setter | Getter |
|  --- | --- | --- | --- | --- |
| X-API-Key | `String` | API key for authentication | `xAPIKey` | `getXAPIKey()` |



**Note:** Auth credentials can be set using `apiKeyCredentials` in the client builder and accessed through `getApiKeyCredentials` method in the client instance.

## Usage Example

### Client Initialization

You must provide credentials in the client as shown in the following code snippet.

```java
import localhost3000.WebhooksAndCallbacksAPIClient;
import localhost3000.authentication.ApiKeyModel;

public class Program {
    public static void main(String[] args) {
        WebhooksAndCallbacksAPIClient client = new WebhooksAndCallbacksAPIClient.Builder()
            .apiKeyCredentials(new ApiKeyModel.Builder(
                    "X-API-Key"
                )
                .build())
            .build();
    }
}
```


