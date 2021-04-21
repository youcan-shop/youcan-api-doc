# Approve a Product Review

Endpoint: `https://api.youcan.shop/reviews/{id}/approve` 

Method: `PUT`

## Parameters

- `id`: Review id

## Response

[200] Review successfully approved

```json
{
    "message": "Product review approved successfully",
    "http_code": 200,
    "code": "UPDATED",
    "type": "success",
    "data": null
}
```

[422] Review already approved

```json
{
    "status": 422,
    "code": "PRODUCT-REVIEW-ALREADY-APPROVED",
    "detail": "Review is already approved.",
    "meta": []
}
```

[404] Review not found