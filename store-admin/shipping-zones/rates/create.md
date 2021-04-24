# Create a Shipping Rate

Endpoint: `https://api.youcan.shop/shipping-zones/{id}/rates`

Method: `POST`

<a name="parameters"></a>

## Parameters

## ShippingRate

| Param Name     | Param Type | Description                   | Required |
| -------------- | ---------- | ----------------------------- | -------- |
| `rates`        | array      | shipping zone rates           | no       |
| `rates.*.min`  | float      | shipping rate min             | yes      |
| `rates.*.max`  | float,null | shipping rate max             | no       |
| `rates.*.price`| float      | shipping rate price           | yes      |

<a name="response"></a>
## Response

[200] OK

```json
{
    "id": "b16556ca-5913-4c90-a2eb-5b5528df0060",
    "name": "Shipping Zone  - Worldwide",
    "display_name": "Shipping Zone  - Worldwide",
    "countries": [
        "rotw"
    ],
    "is_free": false,
    "is_active": true,
    "rate_type": "price",
    "rates": [
        {
            "id": "8773c463-4c3f-4307-87d5-e3671b446775",
            "min": 10.1,
            "max": 20,
            "price": 20
        },
        {
            "id": "af4fad6c-b394-4fb8-8792-7ac56c7f8f2b",
            "min": 0,
            "max": 10,
            "price": 10
        },
        {
            "id": "be73c6bf-4285-408d-9115-6839576b9ed2",
            "min": 20.1,
            "max": 30,
            "price": 30
        },
        {
            "id": "c8af56ee-1c76-4c31-85ff-08e865b8a4ae",
            "min": 30.1,
            "max": null,
            "price": 30.1
        }
    ]
}
```
