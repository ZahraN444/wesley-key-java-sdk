
# Client Class Documentation

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| defaultHost | `String` | *Default*: `"www.example.com"` |
| environment | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](../doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |

The API client can be initialized as follows:

```java
import com.example.www.CypressTestAPIClient;
import com.example.www.Environment;
import com.example.www.exceptions.ApiException;
import java.io.IOException;

public class Program {
    public static void main(String[] args) {
        CypressTestAPIClient client = new CypressTestAPIClient.Builder()
            .httpClientConfig(configBuilder -> configBuilder
                    .timeout(0))
            .environment(Environment.PRODUCTION)
            .defaultHost("www.example.com")
            .build();

    }
}
```

## Cypress Test APIClient Class

The gateway for the SDK. This class acts as a factory for the Controllers and also holds the configuration of the SDK.

### Controllers

| Name | Description | Return Type |
|  --- | --- | --- |
| `getAPIController()` | Provides access to Client controller. | `APIController` |

### Methods

| Name | Description | Return Type |
|  --- | --- | --- |
| `shutdown()` | Shutdown the underlying HttpClient instance. | `void` |
| `getEnvironment()` | Current API environment. | `Environment` |
| `getDefaultHost()` | defaultHost value. | `String` |
| `getHttpClient()` | The HTTP Client instance to use for making HTTP requests. | `HttpClient` |
| `getHttpClientConfig()` | Http Client Configuration instance. | [`ReadonlyHttpClientConfiguration`](../doc/http-client-configuration.md) |
| `getBaseUri(Server server)` | Get base URI by current environment | `String` |
| `getBaseUri()` | Get base URI by current environment | `String` |

