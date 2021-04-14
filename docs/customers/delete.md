# Delete a Customer

Endpoint: `https://api.youcan.shop/customers/{id}`

Method: `DELETE`

<a name="reponse"></a>
## Response

[200] OK
 
```json
{
    "message": "customer successfully deleted",
    "http_code": 200,
    "code": "DELETED",
    "type": "success"
}
```

[400] Bad Request

```json
{
    "status": 400,
    "code": "",
    "detail": "could not delete customer",
    "meta": []
}
```
