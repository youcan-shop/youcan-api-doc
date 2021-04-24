# Delete a Product Review

Endpoint: `https://api.youcan.shop/reviews/{id}` 

Method: `DELETE`

## URL Parameters

- `id`: Review id

## Responses

[200] Review successfully deleted

```json
{
    "message": "Product review deleted successfully",
    "http_code": 200,
    "code": "DELETED",
    "type": "success"
}
```

[404] Review not found
