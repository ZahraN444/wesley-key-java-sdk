# User

Operations about user

```java
UserApi userApi = client.getUserApi();
```

## Class Name

`UserApi`

## Methods

* [Create User](../../doc/controllers/user.md#create-user)
* [Create Users with List Input](../../doc/controllers/user.md#create-users-with-list-input)
* [Login User](../../doc/controllers/user.md#login-user)
* [Logout User](../../doc/controllers/user.md#logout-user)
* [Get User by Name](../../doc/controllers/user.md#get-user-by-name)
* [Update User](../../doc/controllers/user.md#update-user)
* [Delete User](../../doc/controllers/user.md#delete-user)


# Create User

This can only be done by the logged in user.

:information_source: **Note** This endpoint does not require authentication.

```java
CompletableFuture<ApiResponse<User>> createUserAsync(
    final Long id,
    final String username,
    final String firstName,
    final String lastName,
    final String email,
    final String password,
    final String phone,
    final Integer userStatus)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `Long` | Form, Optional | - |
| `username` | `String` | Form, Optional | - |
| `firstName` | `String` | Form, Optional | - |
| `lastName` | `String` | Form, Optional | - |
| `email` | `String` | Form, Optional | - |
| `password` | `String` | Form, Optional | - |
| `phone` | `String` | Form, Optional | - |
| `userStatus` | `Integer` | Form, Optional | User Status |

## Response Type

**200**: successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`User`](../../doc/models/user.md).

## Example Usage

```java
Long id = 10L;
String username = "theUser";
String firstName = "John";
String lastName = "James";
String email = "john@email.com";
String password = "12345";
String phone = "12345";
Integer userStatus = 1;

userApi.createUserAsync(id, username, firstName, lastName, email, password, phone, userStatus).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| Default | Unexpected error | `ApiException` |


# Create Users with List Input

Creates list of users with given input array.

:information_source: **Note** This endpoint does not require authentication.

```java
CompletableFuture<ApiResponse<User>> createUsersWithListInputAsync(
    final List<User> body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`List<User>`](../../doc/models/user.md) | Body, Optional | - |

## Response Type

**200**: Successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`User`](../../doc/models/user.md).

## Example Usage

```java
List<User> body = Arrays.asList(
    new User.Builder()
        .build()
);

userApi.createUsersWithListInputAsync(body).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| Default | Unexpected error | `ApiException` |


# Login User

Log into the system.

:information_source: **Note** This endpoint does not require authentication.

```java
CompletableFuture<ApiResponse<String>> loginUserAsync(
    final String username,
    final String password)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `username` | `String` | Query, Optional | The user name for login |
| `password` | `String` | Query, Optional | The password for login in clear text |

## Response Type

**200**: successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type `String`.

## Example Usage

```java
userApi.loginUserAsync(null, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | Invalid username/password supplied | `ApiException` |
| Default | Unexpected error | `ApiException` |


# Logout User

Log user out of the system.

:information_source: **Note** This endpoint does not require authentication.

```java
CompletableFuture<ApiResponse<Void>> logoutUserAsync()
```

## Response Type

**200**: successful operation

`void`

## Example Usage

```java
userApi.logoutUserAsync().thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| Default | Unexpected error | `ApiException` |


# Get User by Name

Get user detail based on username.

:information_source: **Note** This endpoint does not require authentication.

```java
CompletableFuture<ApiResponse<User>> getUserByNameAsync(
    final String usersname)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `usersname` | `String` | Template, Required | The username that needs to be processed |

## Response Type

**200**: successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`User`](../../doc/models/user.md).

## Example Usage

```java
String usersname = "usersname0";

userApi.getUserByNameAsync(usersname).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | Invalid username supplied | `ApiException` |
| 404 | User not found | `ApiException` |
| Default | Unexpected error | `ApiException` |


# Update User

This can only be done by the logged in user.

:information_source: **Note** This endpoint does not require authentication.

```java
CompletableFuture<ApiResponse<Void>> updateUserAsync(
    final String usersname,
    final Long id,
    final String username,
    final String firstName,
    final String lastName,
    final String email,
    final String password,
    final String phone,
    final Integer userStatus)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `usersname` | `String` | Template, Required | The username that needs to be processed |
| `id` | `Long` | Form, Optional | - |
| `username` | `String` | Form, Optional | - |
| `firstName` | `String` | Form, Optional | - |
| `lastName` | `String` | Form, Optional | - |
| `email` | `String` | Form, Optional | - |
| `password` | `String` | Form, Optional | - |
| `phone` | `String` | Form, Optional | - |
| `userStatus` | `Integer` | Form, Optional | User Status |

## Response Type

**200**: successful operation

`void`

## Example Usage

```java
String usersname = "usersname0";
Long id = 10L;
String username = "theUser";
String firstName = "John";
String lastName = "James";
String email = "john@email.com";
String password = "12345";
String phone = "12345";
Integer userStatus = 1;

userApi.updateUserAsync(usersname, id, username, firstName, lastName, email, password, phone, userStatus).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | bad request | `ApiException` |
| 404 | user not found | `ApiException` |
| Default | Unexpected error | `ApiException` |


# Delete User

This can only be done by the logged in user.

:information_source: **Note** This endpoint does not require authentication.

```java
CompletableFuture<ApiResponse<Void>> deleteUserAsync(
    final String usersname)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `usersname` | `String` | Template, Required | The username that needs to be processed |

## Response Type

**200**: User deleted

`void`

## Example Usage

```java
String usersname = "usersname0";

userApi.deleteUserAsync(usersname).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | Invalid username supplied | `ApiException` |
| 404 | User not found | `ApiException` |
| Default | Unexpected error | `ApiException` |

