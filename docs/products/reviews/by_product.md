# Listing Product Reviews

Endpoint: `https://api.youcan.shop/products/{id}/reviews` 

Method: `GET`

## URL Parameters

- `id`: Product id

## Sorting

- `sort_field`:
  - `ratings`: Product review ratings stars.
  - `first_name`: Product reviewer's first name.
  - `last_name`: Product reviewer's last name.
  - `created_at`: Product review creation date.

## Responses

[200]

```json
{
    "data": [
        {
            "id": "a7dc238d-6ae8-4ad0-b508-07b1f7292434",
            "ratings": 5,
            "first_name": "Test",
            "last_name": "Test",
            "content": "Waw amazing",
            "images_urls": [],
            "created_at": "2021-04-16T11:23:03+00:00"
        }
    ],
    "meta": {
        "pagination": {
            "total": 1,
            "count": 1,
            "per_page": 10,
            "current_page": 1,
            "total_pages": 1,
            "links": {}
        }
    }
}
```

[404] Product not found
