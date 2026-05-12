
# Payment Callback

*This model accepts additional fields of type Object.*

## Structure

`PaymentCallback`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `OrderId` | `String` | Required | - | String getOrderId() | setOrderId(String orderId) |
| `PaymentStatus` | [`PaymentStatus`](../../doc/models/payment-status.md) | Required | - | PaymentStatus getPaymentStatus() | setPaymentStatus(PaymentStatus paymentStatus) |
| `TransactionId` | `String` | Required | - | String getTransactionId() | setTransactionId(String transactionId) |
| `Amount` | `Double` | Optional | - | Double getAmount() | setAmount(Double amount) |
| `Currency` | `String` | Optional | - | String getCurrency() | setCurrency(String currency) |
| `Timestamp` | `LocalDateTime` | Optional | - | LocalDateTime getTimestamp() | setTimestamp(LocalDateTime timestamp) |
| `FailureReason` | `String` | Optional | Reason for payment failure (if applicable) | String getFailureReason() | setFailureReason(String failureReason) |
| `AdditionalProperties` | `Map<String, Object>` | Optional | - | Object getAdditionalProperty(String key) | additionalProperty(String key, Object value) |

## Example (as JSON)

```json
{
  "orderId": "order_789",
  "paymentStatus": "success",
  "transactionId": "txn_abc123",
  "amount": 59.98,
  "currency": "USD",
  "timestamp": "09/19/2025 10:35:00",
  "failureReason": "failureReason0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

