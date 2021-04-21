# Get a Review

Endpoint: `https://api.youcan.shop/reviews/{id}` 

Method: `Get`

## Parameters

- `id`: Review id

## Response

[200]

```json
{
    "id": "e5d50f40-6f2a-4e01-937a-f39da996f56e",
    "ratings": 3,
    "first_name": "Mohamed",
    "last_name": "",
    "content": "",
    "images_urls": [],
    "created_at": "2021-04-21T12:08:46+00:00"
}
```

[404] Review not found