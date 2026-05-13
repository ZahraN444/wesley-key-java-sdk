# Store

Access to Petstore orders

Find out more about our store: [https://swagger.io](https://swagger.io)

```java
StoreApi storeApi = client.getStoreApi();
```

## Class Name

`StoreApi`

## Methods

* [Get Inventory](../../doc/controllers/store.md#get-inventory)
* [Place Order](../../doc/controllers/store.md#place-order)
* [Get Order by Id](../../doc/controllers/store.md#get-order-by-id)
* [Delete Order](../../doc/controllers/store.md#delete-order)


# Get Inventory

Returns a map of status codes to quantities.

```java
CompletableFuture<ApiResponse<Map<String, Integer>>> getInventoryAsync()
```

## Authentication

This endpoint requires [api_key](../../doc/auth/custom-header-signature.md)

## Response Type

**200**: successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type `Map<String, Integer>`.

## Example Usage

```java
storeApi.getInventoryAsync().thenAccept(result -> {
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


# Place Order

Place a new order in the store.

:information_source: **Note** This endpoint does not require authentication.

```java
CompletableFuture<ApiResponse<Order>> placeOrderAsync(
    final Long id,
    final Long petId,
    final Integer quantity,
    final LocalDateTime shipDate,
    final OrderStatus status,
    final Boolean complete)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `Long` | Form, Optional | - |
| `petId` | `Long` | Form, Optional | - |
| `quantity` | `Integer` | Form, Optional | - |
| `shipDate` | `LocalDateTime` | Form, Optional | - |
| `status` | [`OrderStatus`](../../doc/models/order-status.md) | Form, Optional | Order Status |
| `complete` | `Boolean` | Form, Optional | - |

## Response Type

**200**: successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`Order`](../../doc/models/order.md).

## Example Usage

```java
Long id = 10L;
Long petId = 198772L;
Integer quantity = 7;

storeApi.placeOrderAsync(id, petId, quantity, null, null, null).thenAccept(result -> {
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


# Get Order by Id

For valid response try integer IDs with value <= 5 or > 10. Other values will generate exceptions.

:information_source: **Note** This endpoint does not require authentication.

```java
CompletableFuture<ApiResponse<Order>> getOrderByIdAsync(
    final long orderId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `orderId` | `long` | Template, Required | ID of order that needs to be fetched |

## Response Type

**200**: successful operation

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`Order`](../../doc/models/order.md).

## Example Usage

```java
long orderId = 62L;

storeApi.getOrderByIdAsync(orderId).thenAccept(result -> {
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
| 404 | Order not found | `ApiException` |
| Default | Unexpected error | `ApiException` |


# Delete Order

For valid response try integer IDs with value < 1000. Anything above 1000 or non-integers will generate API errors.

:information_source: **Note** This endpoint does not require authentication.

```java
CompletableFuture<ApiResponse<Void>> deleteOrderAsync(
    final long orderId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `orderId` | `long` | Template, Required | ID of the order that needs to be deleted |

## Response Type

**200**: order deleted

`void`

## Example Usage

```java
long orderId = 62L;

storeApi.deleteOrderAsync(orderId).thenAccept(result -> {
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
| 404 | Order not found | `ApiException` |
| Default | Unexpected error | `ApiException` |

