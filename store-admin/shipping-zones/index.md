# Listing Categories

Endpoint: `https://api.youcan.shop/shipping-zones`

Method: `GET`

## Sorting

- `sort field`:
  - `created_at`: Shipping zone creation date

## Response

[200]

```json
{
    "data": [
        {
            "id": "0177319d-29a3-41a6-b0e9-2bce32f4fb62",
            "name": "Fast_Shipping_Worldwide",
            "display_name": "Fast Shipping WorldWide",
            "countries": [
                "rotw"
            ],
            "is_free": false,
            "is_active": true,
            "rate_type": "price",
            "rates": [
                {
                    "id": "42d5a42b-6d10-414c-a1d9-31ce29b53047",
                    "min": 0,
                    "max": 10,
                    "price": 10
                },
                {
                    "id": "89f74b2a-e22e-4485-824c-91e08ae85ec3",
                    "min": 10.1,
                    "max": 20,
                    "price": 20
                },
                {
                    "id": "b21c510c-07db-4b5b-85d9-2e32bc3e3cae",
                    "min": 20.1,
                    "max": 30,
                    "price": 30
                },
                {
                    "id": "cdfc74f8-d0de-43d0-8d14-6feb238825ad",
                    "min": 30.1,
                    "max": null,
                    "price": 30.1
                }
            ]
        },
        {
            "id": "11b314df-124a-4633-afe7-605aaaf446a6",
            "name": "Free_Shipping",
            "display_name": "Free Shipping",
            "countries": [
                "rotw"
            ],
            "is_free": true,
            "is_active": true,
            "rate_type": "price",
            "rates": []
        }
    ],
    "meta": {
        "pagination": {
            "total": 5,
            "count": 5,
            "per_page": 10,
            "current_page": 1,
            "total_pages": 1,
            "links": {}
        }
    }
}
```
