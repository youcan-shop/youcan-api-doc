# Delete a page

Endpoint: `https://api.youcan.shop/pages/{id}`

Method: `DELETE`

## Response

[200] Ok

```json
{
    "message": "Page successfully deleted",
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
    "detail": "Page not found",
    "meta": []
}
```

