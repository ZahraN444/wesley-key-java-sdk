
# Getting Started with Swagger Petstore

## Introduction

This is a sample server Petstore server.  You can find out more about Swagger at [http://swagger.io](http://swagger.io) or on [irc.freenode.net, #swagger](http://swagger.io/irc/).  For this sample, you can use the api key `special-key` to test the authorization filters.

Find out more about Swagger: [http://swagger.io](http://swagger.io)

## Install the Package

Install the SDK by adding the following dependency in your project's pom.xml file:

```xml
<dependency>
  <groupId>io.github.zahran444</groupId>
  <artifactId>wesley-key-sdk</artifactId>
  <version>0.1.7</version>
</dependency>
```

You can also view the package at:
https://central.sonatype.com/artifact/io.github.zahran444/wesley-key-sdk/0.1.7

## Test the SDK

The generated code and the server can be tested using automatically generated test cases.
JUnit is used as the testing framework and test runner.

In Eclipse, for running the tests do the following:

1. Select the project SwaggerPetstoreLib from the package explorer.
2. Select `Run -> Run as -> JUnit Test` or use `Alt + Shift + X` followed by `T` to run the Tests.

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| testHeader | `String` | This is a test header<br>*Default*: `"TestHeaderDefaultValue"` |
| environment | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |
| apiKeyCredentials | [`ApiKeyCredentials`](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/auth/custom-header-signature.md) | The Credentials Setter for Custom Header Signature |
| httpBasicCredentials | [`HttpBasicCredentials`](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/auth/basic-authentication.md) | The Credentials Setter for Basic Authentication |
| petstoreAuthCredentials | [`PetstoreAuthCredentials`](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/auth/oauth-2-implicit-grant.md) | The Credentials Setter for OAuth 2 Implicit Grant |

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

## Environments

The SDK can be configured to use a different environment for making API calls. Available environments are:

### Fields

| Name | Description |
|  --- | --- |
| production | **Default** |
| environment2 | - |
| environment3 | - |

## Authorization

This API uses the following authentication schemes.

* [`api_key (Custom Header Signature)`](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/auth/custom-header-signature.md)
* [`httpBasic (Basic Authentication)`](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/auth/basic-authentication.md)
* [`petstore_auth (OAuth 2 Implicit Grant)`](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/auth/oauth-2-implicit-grant.md)

## List of APIs

* [Pet](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/controllers/pet.md)
* [Store](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/controllers/store.md)
* [User](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/controllers/user.md)

## SDK Infrastructure

### Configuration

* [Configuration Interface](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/configuration-interface.md)
* [HttpClientConfiguration](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/http-client-configuration.md)
* [HttpClientConfiguration.Builder](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/http-client-configuration-builder.md)
* [HttpProxyConfiguration](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/http-proxy-configuration.md)
* [HttpProxyConfiguration.Builder](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/http-proxy-configuration-builder.md)

### HTTP

* [Headers](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/headers.md)
* [HttpCallback Interface](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/http-callback-interface.md)
* [HttpContext](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/http-context.md)
* [HttpBodyRequest](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/http-body-request.md)
* [HttpRequest](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/http-request.md)
* [HttpResponse](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/http-response.md)
* [HttpStringResponse](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/http-string-response.md)

### Utilities

* [ApiException](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/api-exception.md)
* [ApiHelper](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/api-helper.md)
* [FileWrapper](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/file-wrapper.md)
* [DateTimeHelper](https://www.github.com/ZahraN444/wesley-key-java-sdk/tree/0.1.7/doc/date-time-helper.md)

