# Get Seller Profits

Endpoint: `https://api.youcan.shop/profits/{store_id}`

Method :  `GET`

## URL Parameters

- `store_id`: Store id

## Request

`https://api.youcan.shop/profits/2cee434c-2864-4d7b-9e38-fd0b2d5a23cd`

## Response

[200]

```json
{
    "storeEarningsOverview": {
        "today": {
            "earnings": "$ 0",
            "orders_count": 0
        },
        "yesterday": {
            "earnings": "$ 0",
            "orders_count": 0
        },
        "week": {
            "earnings": "$ 0",
            "orders_count": 0
        },
        "month": {
            "earnings": "$ 1280",
            "orders_count": 13
        },
        "year": {
            "earnings": "$ 1280",
            "orders_count": 13
        },
        "all_time": {
            "earnings": "$ 1280",
            "orders_count": 13
        },
        "orders_amount": {
            "average": "$ 98.461538461538",
            "max": "$ 300",
            "min": "$ 10"
        }
    }
}
```