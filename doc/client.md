
# Client Class Documentation

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| testHeader | `String` | This is a test header<br>*Default*: `"TestHeaderDefaultValue"` |
| environment | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](../doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |
| apiKeyCredentials | [`ApiKeyCredentials`](auth/custom-header-signature.md) | The Credentials Setter for Custom Header Signature |
| httpBasicCredentials | [`HttpBasicCredentials`](auth/basic-authentication.md) | The Credentials Setter for Basic Authentication |
| petstoreAuthCredentials | [`PetstoreAuthCredentials`](auth/oauth-2-implicit-grant.md) | The Credentials Setter for OAuth 2 Implicit Grant |

The API client can be initialized as follows:

```java
import io.swagger.petstore.Environment;
import io.swagger.petstore.SwaggerPetstoreClient;
import io.swagger.petstore.authentication.ApiKeyModel;
import io.swagger.petstore.authentication.HttpBasicModel;
import io.swagger.petstore.authentication.PetstoreAuthModel;
import io.swagger.petstore.exceptions.ApiException;
import io.swagger.petstore.models.OAuthScopePetstoreAuthEnum;
import io.swagger.petstore.models.OAuthToken;
import java.io.IOException;
import java.util.Arrays;

public class Program {
    public static void main(String[] args) {
        SwaggerPetstoreClient client = new SwaggerPetstoreClient.Builder()
            .httpClientConfig(configBuilder -> configBuilder
                    .timeout(0))
            .testHeader("TestHeaderDefaultValue")
            .apiKeyCredentials(new ApiKeyModel.Builder(
                    "api_key"
                )
                .build())
            .httpBasicCredentials(new HttpBasicModel.Builder(
                    "username",
                    "passwprd"
                )
                .build())
            .petstoreAuthCredentials(new PetstoreAuthModel.Builder(
                    "OAuthClientId",
                    "OAuthRedirectUri"
                )
                .oAuthScopes(Arrays.asList(
                        OAuthScopePetstoreAuthEnum.READPETS,
                        OAuthScopePetstoreAuthEnum.WRITEPETS
                    ))
                .build())
            .environment(Environment.PRODUCTION)
            .build();

    }
}
```

## Swagger PetstoreClient Class

The gateway for the SDK. This class acts as a factory for the Controllers and also holds the configuration of the SDK.

### Controllers

| Name | Description | Return Type |
|  --- | --- | --- |
| `getPetController()` | Provides access to Pet controller. | `PetController` |
| `getStoreController()` | Provides access to Store controller. | `StoreController` |
| `getUserController()` | Provides access to User controller. | `UserController` |

### Methods

| Name | Description | Return Type |
|  --- | --- | --- |
| `shutdown()` | Shutdown the underlying HttpClient instance. | `void` |
| `getEnvironment()` | Current API environment. | `Environment` |
| `getTestHeader()` | This is a test header. | `String` |
| `getHttpClient()` | The HTTP Client instance to use for making HTTP requests. | `HttpClient` |
| `getHttpClientConfig()` | Http Client Configuration instance. | [`ReadonlyHttpClientConfiguration`](../doc/http-client-configuration.md) |
| `getApiKeyCredentials()` | The credentials to use with ApiKey. | [`ApiKeyCredentials`](auth/custom-header-signature.md) |
| `getHttpBasicCredentials()` | The credentials to use with HttpBasic. | [`HttpBasicCredentials`](auth/basic-authentication.md) |
| `getPetstoreAuthCredentials()` | The credentials to use with PetstoreAuth. | [`PetstoreAuthCredentials`](auth/oauth-2-implicit-grant.md) |
| `getBaseUri(Server server)` | Get base URI by current environment | `String` |
| `getBaseUri()` | Get base URI by current environment | `String` |

