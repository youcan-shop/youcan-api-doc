# Reject a Review

Endpoint: `https://api.youcan.shop/reviews/{id}/reject` 

Method: `PUT`

## Parameters

- `id`: Review id

## Response

[200] Review successfully rejected

```json
{
    "message": "Product review rejected successfully",
    "http_code": 200,
    "code": "UPDATED",
    "type": "success",
    "data": null
}
```

[422] Review already rejected

```json
{
    "status": 422,
    "code": "PRODUCT-REVIEW-ALREADY-REJECTED",
    "detail": "Review is already rejected.",
    "meta": []
}
```

[404] Review not found