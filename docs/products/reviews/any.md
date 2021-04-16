# Listing Products Reviews

Endpoint: `https://api.youcan.shop/reviews` 

Method: `GET`

## Sorting

- `sort_field`:
  - `name`: Product name.
  - `price`: Product price.
  - `orders_count`: Product orders count.
  - `you_save_amount`: The different between price and compare at price.

## Filters

| Field Name | Operator | Value type | Description |
| --- | --- | --- | --- |
| `inventory` | `<`, `<`, `=` | number | Product inventory |



## Response

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
