# Delete a Product

Endpoint: `https://api.youcan.shop/products/{id}`

Method: `DELETE`

## Responses

[200] OK
 
```json
{
    "message": "Product successfully deleted",
    "type": "success"
}
```

[404] Not Found

```json
{
    "status": 404,
    "detail": "Product not found",
    "meta": []
}
```

[500] Internal error

```json
{
    "status": 500,
    "detail": "Internal error",
    "meta": []
}
```
