# Close Order

Endpoint: `https://api.youcan.shop/orders/{id}/close`

Method: `PUT`

Body:

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| cancel_order | boolean | cancel order & return it to stock | no |

## Response

[200] Order successfully closed

```json
{
  "message": "The order closed successfully.",
  "http_code": 200,
  "code": "UPDATED",
  "type": "success",
  "data": null
}
```

[400] Order not closed

```json
{
  "status": 400,
  "code": "ORDER-NOT-CLOSED",
  "detail": "Order #021A not closed.",
  "meta": []
}
```

[422] Order already fulfilled

```json
{
  "status": 422,
  "code": "ORDER-ALREADY-CLOSED",
  "detail": "Order #021A is already closed.",
  "meta": []
}
```