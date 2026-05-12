# Orders

Order management operations

```java
OrdersApi ordersApi = client.getOrdersApi();
```

## Class Name

`OrdersApi`


# Create Order

Creates a new order and triggers callbacks for payment processing

```java
CompletableFuture<ApiResponse<Order>> createOrderAsync(
    final CreateOrderRequest body)
```

## Authentication

This endpoint requires [ApiKey](../../doc/auth/custom-header-signature.md) **OR** [BearerAuth](../../doc/auth/oauth-2-bearer-token.md)

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`CreateOrderRequest`](../../doc/models/create-order-request.md) | Body, Required | - |

## Response Type

**201**: Order created successfully

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` getter of this instance returns the response data which is of type [`Order`](../../doc/models/order.md).

## Related Callbacks

| Name | Description |
|  --- | --- |
| [Payment Callback](../../doc/events/callbacks/callbacks_a/payment-callback.md) | Called when payment processing is complete |
| [Fulfillment Callback](../../doc/events/callbacks/callbacks_a/fulfillment-callback.md) | Called when order processing is complete |
| [Email Notification Callback](../../doc/events/callbacks/callbacks_b/email-notification-callback.md) | Called when email notification delivery is complete |
| [Sms Notification Callback](../../doc/events/callbacks/callbacks_b/sms-notification-callback.md) | Called when SMS notification delivery is complete |

## Example Usage

```java
CreateOrderRequest body = new CreateOrderRequest.Builder(
    "cust_12345",
    Arrays.asList(
        new OrderItem.Builder(
            "prod_001",
            2,
            29.99D
        )
        .build()
    ),
    "https://merchant.example.com/callbacks/payment"
)
.build();

ordersApi.createOrderAsync(body).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    Throwable cause = exception.getCause();

    if (cause instanceof ErrorException) {
        ErrorException errorException = (ErrorException) cause;
        errorException.printStackTrace();
    } else {
        // fallback for unexpected errors
        exception.printStackTrace();
    }

    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | Invalid request | [`ErrorException`](../../doc/models/error-exception.md) |

