# Listing Products Reviews

Endpoint: `https://my-store.com/api/products/{id}/reviews` 

Method: `GET`

## Sorting

- `sort_field`:
  - `first_name`: Reviewer first name.
  - `last_name`: Reviewer last name.
  - `email`: Reviewer email.
  - `ratings`: Reviewer rating.
  - `created_at`: Creation date.

## Response

[200]

```json
{
    "data": [
        {
            "id": "64109e6e-03dc-4ae2-9187-9b584b28a024",
            "ratings": 5,
            "first_name": "Zephr",
            "last_name": "Hurley",
            "content": "Eum ut et beatae arc",
            "images_urls": ["http://cdn.dotshop.com/stores/afnisse/products/gnuYpd98X6huXaR51aL8GO23IYnERB08KUMOhdLA_md.jpeg"],
            "created_at": "2020-12-07T16:58:54+00:00"
        },
        {
            "id": "912d8761-d1c1-4555-829d-5407dbd3bf01",
            "ratings": 4,
            "first_name": "Quentin",
            "last_name": "Vazquez",
            "content": "Dolorem nihil est vo",
            "images_urls": [],
            "created_at": "2020-12-07T16:58:05+00:00"
        }
    ],
    "meta": {
        "pagination": {
            "total": 2,
            "count": 2,
            "per_page": 10,
            "current_page": 1,
            "total_pages": 1,
            "links": {}
        }
    }
}
```
