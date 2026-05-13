
# Client Class Documentation

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | [`Environment`](../README.md#environments) | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](../doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |
| loggingConfig | [`Consumer<ApiLoggingConfiguration.Builder>`](../doc/api-logging-configuration-builder.md) | Set up Logging Configuration instance. |
| petstoreAuthCredentials | [`PetstoreAuthCredentials`](auth/oauth-2-implicit-grant.md) | The Credentials Setter for OAuth 2 Implicit Grant |
| apiKeyCredentials | [`ApiKeyCredentials`](auth/custom-header-signature.md) | The Credentials Setter for Custom Header Signature |

The API client can be initialized as follows:

```java
import io.swagger.petstore3.Environment;
import io.swagger.petstore3.SwaggerPetstoreOpenApi30Client;
import io.swagger.petstore3.authentication.ApiKeyModel;
import io.swagger.petstore3.authentication.PetstoreAuthModel;
import io.swagger.petstore3.exceptions.ApiException;
import io.swagger.petstore3.http.response.ApiResponse;
import io.swagger.petstore3.models.OauthScopePetstoreAuth;
import io.swagger.petstore3.models.OauthToken;
import java.io.IOException;
import java.util.Arrays;
import javax.xml.bind.JAXBException;
import org.slf4j.event.Level;

public class Program {
    public static void main(String[] args) {
        SwaggerPetstoreOpenApi30Client client = new SwaggerPetstoreOpenApi30Client.Builder()
            .loggingConfig(builder -> builder
                    .level(Level.DEBUG)
                    .requestConfig(logConfigBuilder -> logConfigBuilder.body(true))
                    .responseConfig(logConfigBuilder -> logConfigBuilder.headers(true)))
            .httpClientConfig(configBuilder -> configBuilder
                    .timeout(0))
            .petstoreAuthCredentials(new PetstoreAuthModel.Builder(
                    "OAuthClientId",
                    "OAuthRedirectUri"
                )
                .oauthScopes(Arrays.asList(
                        OauthScopePetstoreAuth.WRITEPETS,
                        OauthScopePetstoreAuth.READPETS
                    ))
                .build())
            .apiKeyCredentials(new ApiKeyModel.Builder(
                    "api_key"
                )
                .build())
            .environment(Environment.PRODUCTION)
            .build();

    }
}
```

## Swagger Petstore - OpenAPI 3.0Client Class

The gateway for the SDK. This class acts as a factory for the Apis and also holds the configuration of the SDK.

### Apis

| Name | Description | Return Type |
|  --- | --- | --- |
| `getPetApi()` | Provides access to Pet controller. | `PetApi` |
| `getStoreApi()` | Provides access to Store controller. | `StoreApi` |
| `getUserApi()` | Provides access to User controller. | `UserApi` |

### Methods

| Name | Description | Return Type |
|  --- | --- | --- |
| `shutdown()` | Shutdown the underlying HttpClient instance. | `void` |
| `getEnvironment()` | Current API environment. | `Environment` |
| `getHttpClient()` | The HTTP Client instance to use for making HTTP requests. | `HttpClient` |
| `getHttpClientConfig()` | Http Client Configuration instance. | [`ReadonlyHttpClientConfiguration`](../doc/http-client-configuration.md) |
| `getLoggingConfig()` | Logging Configuration instance. | [`ReadonlyLoggingConfiguration`](../doc/api-logging-configuration.md) |
| `getPetstoreAuthCredentials()` | The credentials to use with PetstoreAuth. | [`PetstoreAuthCredentials`](auth/oauth-2-implicit-grant.md) |
| `getApiKeyCredentials()` | The credentials to use with ApiKey. | [`ApiKeyCredentials`](auth/custom-header-signature.md) |
| `getBaseUri(Server server)` | Get base URI by current environment | `String` |
| `getBaseUri()` | Get base URI by current environment | `String` |

