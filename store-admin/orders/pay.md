# Mark Order As paid

Endpoint: `https://api.youcan.shop/orders/{id}/pay`

Method: `PUT`

## Response

[200] Order successfully closed

```json
{
  "message": "The order is paid successfully.",
  "type": "success",
  "data": null
}
```

[404] Order not found

```json
{
  "status": 404,
  "detail": "order not found",
  "meta": []
}
```

[422] Order already paid

```json
{
  "status": 422,
  "detail": "Order #298 is already paid.",
  "meta": []
}
```