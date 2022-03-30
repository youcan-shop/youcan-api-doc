# Get Seller Profits

Endpoint: `https://api.youcan.shop/stores/profit`

Method :  `GET`

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