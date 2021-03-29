# Fulfill Order

Endpoint: `https://seller-area.youcan.shop/admin/api/orders/{id}/fulfill`

Method: `PUT`

Body:

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| seller_note | string | note from the seller | no |
| tracking_number | string | shipping tracking number | no |

## Response

[200] Order successfully fulfilled

```json
{
  "message": "The order is fulfilled successfully.",
  "http_code": 200,
  "code": "UPDATED",
  "type": "success",
  "data": null
}
```

[422] Order already fulfilled

```json
{
  "status": 422,
  "code": "ORDER-ALREADY-FULFILLED",
  "detail": "Order #021A is already fulfilled.",
  "meta": []
}
```