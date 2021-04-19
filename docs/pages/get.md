# Get a page

Endpoint: `https://api.youcan.shop/pages/{id}`

Method: `GET`

## Response

[200] Ok

```json
{
    "id": "11f81fc2-ce46-4f44-896b-d6cf26504635",
    "name": "about-us",
    "slug": "about-us",
    "visibility": "1",
    "public_url": "http://azizi.dotshop.com/pages/about-us",
    "content": "<h4>about us</h4>",
    "created_at": "2021-04-19T12:33:50+00:00",
    "meta": {
        "title": "about us",
        "description": "about us description",
        "images": []
    }
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

