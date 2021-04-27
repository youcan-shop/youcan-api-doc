# Delete a Shipping Zone

Endpoint: `https://api.youcan.shop/shipping-zones/{id}`

Method: `DELETE`

<a name="response"></a>

## Response

[200] OK
 
```json
{
    "message": "Shipping zone successfully deleted",
    "http_code": 200,
    "code": "DELETED",
    "type": "success"
}
```

[404] Not Found
 
```json
{
    "status": 404,
    "code": 404,
    "detail": "Shipping zone not found",
    "meta": []
}
```

