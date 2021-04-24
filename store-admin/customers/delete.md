# Delete a Customer

Endpoint: `https://api.youcan.shop/customers/{id}`

Method: `DELETE`

<a name="response"></a>

## Responses

[200] OK
 
```json
{
    "message": "customer successfully deleted",
    "http_code": 200,
    "code": "DELETED",
    "type": "success"
}
```

[404] Not Found

```json
{
    "status": 404,
    "code": 0,
    "detail": "Customer not found",
    "meta": []
}
```
