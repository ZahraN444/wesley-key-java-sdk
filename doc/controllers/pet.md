# Pet

Everything about your Pets

Find out more: [https://swagger.io](https://swagger.io)

```java
PetApi petApi = client.getPetApi();
```

## Class Name

`PetApi`

## Methods

* [Update Pet](../../doc/controllers/pet.md#update-pet)
* [Add Pet](../../doc/controllers/pet.md#add-pet)
* [Find Pets by Status](../../doc/controllers/pet.md#find-pets-by-status)
* [Find Pets by Tags](../../doc/controllers/pet.md#find-pets-by-tags)
* [Get Pet by Id](../../doc/controllers/pet.md#get-pet-by-id)
* [Update Pet with Form](../../doc/controllers/pet.md#update-pet-with-form)
* [Delete Pet](../../doc/controllers/pet.md#delete-pet)
* [Upload File](../../doc/controllers/pet.md#upload-file)


# Update Pet

Update an existing pet by Id.

```java
CompletableFuture<ApiResponse<Pet>> updatePetAsync(
    final String name,
    final List<String> photoUrls,
    final Long id,
    final Category category,
    final List<Tag> tags,
    final PetStatus status)
```

## Authentication

This endpoint requires [petstore_auth](../../doc/auth/oauth-2-implicit-grant.md)

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `name` | `String` | Form, Required | - |
| `photoUrls` | `List<String>` | Form, Required | - |
| `id` | `Long` | Form, Optional | - |
| `category` | [`Category`](../../doc/models/category.md) | Form, Optional | - |
| `tags` | [`List<Tag>`](../../doc/models/tag.md) | Form, Optional | - |
| `status` | [`PetStatus`](../../doc/models/pet-status.md) | Form, Optional | pet status in the store |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

**200**: Successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`Pet`](../../doc/models/pet.md).

## Example Usage

```java
String name = "doggie";
List<String> photoUrls = Arrays.asList(
    "photoUrls5",
    "photoUrls6",
    "photoUrls7"
);

Long id = 10L;
List<Tag> tags = Arrays.asList(
    new Tag.Builder()
        .build()
);


petApi.updatePetAsync(name, photoUrls, id, null, tags, null).thenAccept(result -> {
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
| 400 | Invalid ID supplied | `ApiException` |
| 404 | Pet not found | `ApiException` |
| 422 | Validation exception | `ApiException` |
| Default | Unexpected error | `ApiException` |


# Add Pet

Add a new pet to the store.

```java
CompletableFuture<ApiResponse<Pet>> addPetAsync(
    final String name,
    final List<String> photoUrls,
    final Long id,
    final Category category,
    final List<Tag> tags,
    final PetStatus status)
```

## Authentication

This endpoint requires [petstore_auth](../../doc/auth/oauth-2-implicit-grant.md)

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `name` | `String` | Form, Required | - |
| `photoUrls` | `List<String>` | Form, Required | - |
| `id` | `Long` | Form, Optional | - |
| `category` | [`Category`](../../doc/models/category.md) | Form, Optional | - |
| `tags` | [`List<Tag>`](../../doc/models/tag.md) | Form, Optional | - |
| `status` | [`PetStatus`](../../doc/models/pet-status.md) | Form, Optional | pet status in the store |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

**200**: Successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`Pet`](../../doc/models/pet.md).

## Example Usage

```java
String name = "doggie";
List<String> photoUrls = Arrays.asList(
    "photoUrls5",
    "photoUrls6",
    "photoUrls7"
);

Long id = 10L;
List<Tag> tags = Arrays.asList(
    new Tag.Builder()
        .build()
);


petApi.addPetAsync(name, photoUrls, id, null, tags, null).thenAccept(result -> {
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
| 400 | Invalid input | `ApiException` |
| 422 | Validation exception | `ApiException` |
| Default | Unexpected error | `ApiException` |


# Find Pets by Status

Multiple status values can be provided with comma separated strings.

```java
CompletableFuture<ApiResponse<List<Pet>>> findPetsByStatusAsync(
    final PetStatus status)
```

## Authentication

This endpoint requires [petstore_auth](../../doc/auth/oauth-2-implicit-grant.md)

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `status` | [`PetStatus`](../../doc/models/pet-status.md) | Query, Optional | Status values that need to be considered for filter |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

**200**: successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`List<Pet>`](../../doc/models/pet.md).

## Example Usage

```java
petApi.findPetsByStatusAsync(null).thenAccept(result -> {
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
| 400 | Invalid status value | `ApiException` |
| Default | Unexpected error | `ApiException` |


# Find Pets by Tags

Multiple tags can be provided with comma separated strings. Use tag1, tag2, tag3 for testing.

```java
CompletableFuture<ApiResponse<List<Pet>>> findPetsByTagsAsync(
    final List<String> tags)
```

## Authentication

This endpoint requires [petstore_auth](../../doc/auth/oauth-2-implicit-grant.md)

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `tags` | `List<String>` | Query, Optional | Tags to filter by |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

**200**: successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`List<Pet>`](../../doc/models/pet.md).

## Example Usage

```java
petApi.findPetsByTagsAsync(null).thenAccept(result -> {
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
| 400 | Invalid tag value | `ApiException` |
| Default | Unexpected error | `ApiException` |


# Get Pet by Id

Returns a single pet.

```java
CompletableFuture<ApiResponse<Pet>> getPetByIdAsync(
    final long petId)
```

## Authentication

This endpoint requires [api_key](../../doc/auth/custom-header-signature.md) **OR** [petstore_auth](../../doc/auth/oauth-2-implicit-grant.md)

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `petId` | `long` | Template, Required | ID of pet to return |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

**200**: successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`Pet`](../../doc/models/pet.md).

## Example Usage

```java
long petId = 10L;

petApi.getPetByIdAsync(petId).thenAccept(result -> {
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
| 400 | Invalid ID supplied | `ApiException` |
| 404 | Pet not found | `ApiException` |
| Default | Unexpected error | `ApiException` |


# Update Pet with Form

Updates a pet resource based on the form data.

```java
CompletableFuture<ApiResponse<Pet>> updatePetWithFormAsync(
    final long petId,
    final String name,
    final String status)
```

## Authentication

This endpoint requires [petstore_auth](../../doc/auth/oauth-2-implicit-grant.md)

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `petId` | `long` | Template, Required | ID of pet that needs to be updated |
| `name` | `String` | Query, Optional | Name of pet that needs to be updated |
| `status` | `String` | Query, Optional | Status of pet that needs to be updated |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

**200**: successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`Pet`](../../doc/models/pet.md).

## Example Usage

```java
long petId = 10L;

petApi.updatePetWithFormAsync(petId, null, null).thenAccept(result -> {
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
| 400 | Invalid input | `ApiException` |
| Default | Unexpected error | `ApiException` |


# Delete Pet

Delete a pet.

```java
CompletableFuture<ApiResponse<Void>> deletePetAsync(
    final long petId,
    final String apiKey)
```

## Authentication

This endpoint requires [petstore_auth](../../doc/auth/oauth-2-implicit-grant.md)

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `petId` | `long` | Template, Required | Pet id to delete |
| `apiKey` | `String` | Header, Optional | - |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

**200**: Pet deleted

`void`

## Example Usage

```java
long petId = 10L;

petApi.deletePetAsync(petId, null).thenAccept(result -> {
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
| 400 | Invalid pet value | `ApiException` |
| Default | Unexpected error | `ApiException` |


# Upload File

Upload image of the pet.

```java
CompletableFuture<ApiResponse<ApiResponse>> uploadFileAsync(
    final long petId,
    final String additionalMetadata,
    final FileWrapper body)
```

## Authentication

This endpoint requires [petstore_auth](../../doc/auth/oauth-2-implicit-grant.md)

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `petId` | `long` | Template, Required | ID of pet to update |
| `additionalMetadata` | `String` | Query, Optional | Additional Metadata |
| `body` | `FileWrapper` | Form, Optional | - |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

**200**: successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`ApiResponse`](../../doc/models/api-response.md).

## Example Usage

```java
long petId = 10L;

petApi.uploadFileAsync(petId, null, null).thenAccept(result -> {
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
| 400 | No file uploaded | `ApiException` |
| 404 | Pet not found | `ApiException` |
| Default | Unexpected error | `ApiException` |

