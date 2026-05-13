
# Getting Started with Swagger Petstore - OpenAPI 3.0

## Introduction

This is a sample Pet Store Server based on the OpenAPI 3.0 specification.  You can find out more about
Swagger at [https://swagger.io](https://swagger.io). In the third iteration of the pet store, we've switched to the design first approach!
You can now help us improve the API whether it's by making changes to the definition itself or to the code.
That way, with time, we can improve the API in general, and expose some of the new features in OAS3.

Some useful links:

- [The Pet Store repository](https://github.com/swagger-api/swagger-petstore)
- [The source API definition for the Pet Store](https://github.com/swagger-api/swagger-petstore/blob/master/src/main/resources/openapi.yaml)

Find out more about Swagger: [https://swagger.io](https://swagger.io)

## Install the Package

Install the SDK by adding the following dependency in your project's pom.xml file:

```xml
<dependency>
  <groupId>io.github.zahran444</groupId>
  <artifactId>wesley-key-sdk</artifactId>
  <version>4.0.2</version>
</dependency>
```

You can also view the package at:
https://central.sonatype.com/artifact/io.github.zahran444/wesley-key-sdk/4.0.2

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | [`Environment`](README.md#environments) | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |
| loggingConfig | [`Consumer<ApiLoggingConfiguration.Builder>`](doc/api-logging-configuration-builder.md) | Set up Logging Configuration instance. |
| petstoreAuthCredentials | [`PetstoreAuthCredentials`](doc/auth/oauth-2-implicit-grant.md) | The Credentials Setter for OAuth 2 Implicit Grant |
| apiKeyCredentials | [`ApiKeyCredentials`](doc/auth/custom-header-signature.md) | The Credentials Setter for Custom Header Signature |

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

## Environments

The SDK can be configured to use a different environment for making API calls. Available environments are:

### Fields

| Name | Description |
|  --- | --- |
| PRODUCTION | **Default** |

## Authorization

This API uses the following authentication schemes.

* [`petstore_auth (OAuth 2 Implicit Grant)`](doc/auth/oauth-2-implicit-grant.md)
* [`api_key (Custom Header Signature)`](doc/auth/custom-header-signature.md)

## List of APIs

* [Pet](doc/controllers/pet.md)
* [Store](doc/controllers/store.md)
* [User](doc/controllers/user.md)

## SDK Infrastructure

### Configuration

* [ApiLoggingConfiguration](doc/api-logging-configuration.md)
* [ApiLoggingConfiguration.Builder](doc/api-logging-configuration-builder.md)
* [ApiRequestLoggingConfiguration.Builder](doc/api-request-logging-configuration-builder.md)
* [ApiResponseLoggingConfiguration.Builder](doc/api-response-logging-configuration-builder.md)
* [Configuration Interface](doc/configuration-interface.md)
* [HttpClientConfiguration](doc/http-client-configuration.md)
* [HttpClientConfiguration.Builder](doc/http-client-configuration-builder.md)
* [HttpProxyConfiguration](doc/http-proxy-configuration.md)
* [HttpProxyConfiguration.Builder](doc/http-proxy-configuration-builder.md)

### HTTP

* [Headers](doc/headers.md)
* [HttpCallback Interface](doc/http-callback-interface.md)
* [HttpContext](doc/http-context.md)
* [HttpBodyRequest](doc/http-body-request.md)
* [HttpRequest](doc/http-request.md)
* [HttpResponse](doc/http-response.md)
* [HttpStringResponse](doc/http-string-response.md)

### Utilities

* [ApiException](doc/api-exception.md)
* [ApiResponse](doc/api-response.md)
* [ApiHelper](doc/api-helper.md)
* [FileWrapper](doc/file-wrapper.md)
* [DateTimeHelper](doc/date-time-helper.md)

