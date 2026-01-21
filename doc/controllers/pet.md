# Pet

Everything about your Pets

Find out more: [http://swagger.io](http://swagger.io)

```java
PetController petController = client.getPetController();
```

## Class Name

`PetController`

## Methods

* [Get Pet by Id](../../doc/controllers/pet.md#get-pet-by-id)
* [Update Pet With Form](../../doc/controllers/pet.md#update-pet-with-form)
* [Delete Pet](../../doc/controllers/pet.md#delete-pet)
* [Add Pet](../../doc/controllers/pet.md#add-pet)
* [Update Pet](../../doc/controllers/pet.md#update-pet)
* [Find Pets by Status](../../doc/controllers/pet.md#find-pets-by-status)
* [Upload File](../../doc/controllers/pet.md#upload-file)
* [Find Pets by Tags](../../doc/controllers/pet.md#find-pets-by-tags)


# Get Pet by Id

Returns a single pet

```java
CompletableFuture<Pet> getPetByIdAsync(
    final long petId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `petId` | `long` | Template, Required | ID of pet to return |

## Response Type

[`Pet`](../../doc/models/pet.md)

## Example Usage

```java
long petId = 152L;

petController.getPetByIdAsync(petId).thenAccept(result -> {
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


# Update Pet With Form

Updates a pet in the store with form data

```java
CompletableFuture<Void> updatePetWithFormAsync(
    final long petId,
    final ContentTypeEnum contentType,
    final String name,
    final String status)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `petId` | `long` | Template, Required | ID of pet that needs to be updated |
| `contentType` | [`ContentTypeEnum`](../../doc/models/content-type-enum.md) | Header, Required | - |
| `name` | `String` | Form, Optional | Updated name of the pet |
| `status` | `String` | Form, Optional | Updated status of the pet |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

`void`

## Example Usage

```java
long petId = 152L;
ContentTypeEnum contentType = ContentTypeEnum.ENUM_APPLICATIONXWWWFORMURLENCODED;

petController.updatePetWithFormAsync(petId, contentType, null, null).thenAccept(result -> {
    // TODO success callback handler
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 405 | Invalid input | `ApiException` |


# Delete Pet

Deletes a pet

```java
CompletableFuture<Void> deletePetAsync(
    final long petId,
    final String apiKey)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `petId` | `long` | Template, Required | Pet id to delete |
| `apiKey` | `String` | Header, Optional | - |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

`void`

## Example Usage

```java
long petId = 152L;

petController.deletePetAsync(petId, null).thenAccept(result -> {
    // TODO success callback handler
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


# Add Pet

Add a new pet to the store

```java
CompletableFuture<Void> addPetAsync(
    final PetRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`PetRequest`](../../doc/models/pet-request.md) | Body, Required | Pet object that needs to be added to the store |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

`void`

## Example Usage

```java
PetRequest body = new PetRequest.Builder(
    "name6",
    Arrays.asList(
        "photoUrls1"
    )
)
.build();

petController.addPetAsync(body).thenAccept(result -> {
    // TODO success callback handler
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 405 | Invalid input | `ApiException` |


# Update Pet

Update an existing pet

```java
CompletableFuture<Void> updatePetAsync(
    final PetRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`PetRequest`](../../doc/models/pet-request.md) | Body, Required | Pet object that needs to be added to the store |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

`void`

## Example Usage

```java
PetRequest body = new PetRequest.Builder(
    "name6",
    Arrays.asList(
        "photoUrls1"
    )
)
.build();

petController.updatePetAsync(body).thenAccept(result -> {
    // TODO success callback handler
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
| 405 | Validation exception | `ApiException` |


# Find Pets by Status

Multiple status values can be provided with comma separated strings

```java
CompletableFuture<List<Pet>> findPetsByStatusAsync(
    final List<Status2Enum> status)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `status` | [`List<Status2Enum>`](../../doc/models/status-2-enum.md) | Query, Required | Status values that need to be considered for filter |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

[`List<Pet>`](../../doc/models/pet.md)

## Example Usage

```java
List<Status2Enum> status = Arrays.asList(
    Status2Enum.PENDING,
    Status2Enum.SOLD,
    Status2Enum.AVAILABLE
);

petController.findPetsByStatusAsync(status).thenAccept(result -> {
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


# Upload File

uploads an image

```java
CompletableFuture<ApiResponse> uploadFileAsync(
    final long petId,
    final String additionalMetadata,
    final FileWrapper file)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `petId` | `long` | Template, Required | ID of pet to update |
| `additionalMetadata` | `String` | Form, Optional | Additional data to pass to server |
| `file` | `FileWrapper` | Form, Optional | file to upload |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

[`ApiResponse`](../../doc/models/api-response.md)

## Example Usage

```java
long petId = 152L;

petController.uploadFileAsync(petId, null, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```


# Find Pets by Tags

**This endpoint is deprecated.**

Multiple tags can be provided with comma separated strings. Use tag1, tag2, tag3 for testing.

```java
CompletableFuture<List<Pet>> findPetsByTagsAsync(
    final List<String> tags)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `tags` | `List<String>` | Query, Required | Tags to filter by |

## Requires scope

### petstore_auth

`read:pets`, `write:pets`

## Response Type

[`List<Pet>`](../../doc/models/pet.md)

## Example Usage

```java
List<String> tags = Arrays.asList(
    "tags5",
    "tags6"
);

petController.findPetsByTagsAsync(tags).thenAccept(result -> {
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

