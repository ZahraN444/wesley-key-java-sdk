
# Basic Authentication



Documentation for accessing and setting credentials for httpBasic.

## Auth Credentials

| Name | Type | Description | Setter | Getter |
|  --- | --- | --- | --- | --- |
| username | `String` | - | `username` | `getUsername()` |
| passwprd | `String` | - | `passwprd` | `getPasswprd()` |



**Note:** Auth credentials can be set using `httpBasicCredentials` in the client builder and accessed through `getHttpBasicCredentials` method in the client instance.

## Usage Example

### Client Initialization

You must provide credentials in the client as shown in the following code snippet.

```java
import io.swagger.petstore.SwaggerPetstoreClient;
import io.swagger.petstore.authentication.HttpBasicModel;

public class Program {
    public static void main(String[] args) {
        SwaggerPetstoreClient client = new SwaggerPetstoreClient.Builder()
            .httpBasicCredentials(new HttpBasicModel.Builder(
                    "username",
                    "passwprd"
                )
                .build())
            .build();
    }
}
```


