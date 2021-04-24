# Get a Shipping Zone

Endpoint: `https://api.youcan.shop/shipping-zones/{id}`

Method: `GET`

## Responses

[200] OK

```json
{
    "id": "b5f5e964-c34a-4e48-90f2-8a1853bc1596",
    "name": "Fast Shipping Worldwide",
    "display_name": "Fast Shipping Worldwide",
    "countries": [
        "rotw"
    ],
    "is_free": false,
    "is_active": true,
    "rate_type": "price",
    "rates": [
        {
            "id": "c1095c02-ad79-4a77-a06c-fa3bad157fcc",
            "min": 20.1,
            "max": 30,
            "price": 30
        },
        {
            "id": "ce7b658a-49ed-4808-9a9c-d768157799f7",
            "min": 10.1,
            "max": 20,
            "price": 20
        },
        {
            "id": "e8558101-d47b-4ec3-b901-e26452f9e9fa",
            "min": 0,
            "max": 10,
            "price": 10
        },
        {
            "id": "feb23f02-3f0d-4cbe-9d4d-bad547723ab6",
            "min": 30.1,
            "max": null,
            "price": 30.1
        }
    ]
}
```

[404] Not Found
 
```json
{
    "status": 404,
    "code": 404,
    "detail": "Shipping zone not found",
    "meta": []
}
```
