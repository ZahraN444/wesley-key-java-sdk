
# Getting Started with Webhooks and Callbacks API

## Introduction

A comprehensive API demonstrating webhooks and callbacks patterns.

### Webhooks

Webhooks allow your application to receive real-time notifications when certain events occur.

### Callbacks

Callbacks are used for asynchronous operations where the API will call back to your provided URL when the operation completes.

## Install the Package

Install the SDK by adding the following dependency in your project's pom.xml file:

```xml
<dependency>
  <groupId>io.github.zahran444</groupId>
  <artifactId>wesley-key-sdk</artifactId>
  <version>4.0.0</version>
</dependency>
```

You can also view the package at:
https://central.sonatype.com/artifact/io.github.zahran444/wesley-key-sdk/4.0.0

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |
| loggingConfig | [`Consumer<ApiLoggingConfiguration.Builder>`](doc/api-logging-configuration-builder.md) | Set up Logging Configuration instance. |
| apiKeyCredentials | [`ApiKeyCredentials`](doc/auth/custom-header-signature.md) | The Credentials Setter for Custom Header Signature |
| bearerAuthCredentials | [`BearerAuthCredentials`](doc/auth/oauth-2-bearer-token.md) | The Credentials Setter for OAuth 2 Bearer token |

The API client can be initialized as follows:

```java
import localhost3000.WebhooksAndCallbacksAPIClient;
import localhost3000.authentication.ApiKeyModel;
import localhost3000.authentication.BearerAuthModel;
import localhost3000.exceptions.ApiException;
import localhost3000.http.response.ApiResponse;
import org.slf4j.event.Level;

public class Program {
    public static void main(String[] args) {
        WebhooksAndCallbacksAPIClient client = new WebhooksAndCallbacksAPIClient.Builder()
            .loggingConfig(builder -> builder
                    .level(Level.DEBUG)
                    .requestConfig(logConfigBuilder -> logConfigBuilder.body(true))
                    .responseConfig(logConfigBuilder -> logConfigBuilder.headers(true)))
            .httpClientConfig(configBuilder -> configBuilder
                    .timeout(0))
            .apiKeyCredentials(new ApiKeyModel.Builder(
                    "X-API-Key"
                )
                .build())
            .bearerAuthCredentials(new BearerAuthModel.Builder(
                    "AccessToken"
                )
                .build())
            .build();

    }
}
```

## Authorization

This API uses the following authentication schemes.

* [`ApiKey (Custom Header Signature)`](doc/auth/custom-header-signature.md)
* [`BearerAuth (OAuth 2 Bearer token)`](doc/auth/oauth-2-bearer-token.md)

## List of APIs

* [Orders](doc/controllers/orders.md)

## Webhooks

* [Webhooks](doc/events/webhooks/webhooks-handler.md)
* [Webhooks A](doc/events/webhooks/webhooks-a-handler.md)
* [Webhooks B](doc/events/webhooks/webhooks-b-handler.md)
* [Webhooks C](doc/events/webhooks/webhooks-c-handler.md)
* [Webhooks No Verification](doc/events/webhooks/webhooks-no-verification-handler.md)

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

