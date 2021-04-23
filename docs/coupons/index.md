# Listing Coupons

Endpoint: `https://api.youcan.shop/coupons` 

Method: `GET`

## Response

[200] Ok

```json
{
    "data": [
        {
            "id": "15211be0-2579-4dde-bec2-25f05086e91f",
            "code": "code0332",
            "description": "coupoun 02 from api",
            "value": 5,
            "type": 1,
            "type_text": "percentage",
            "start_date": 1619308800,
            "end_date": 1619395200,
            "max_usage": 55,
            "status": "Expired"
        },
        {
            "id": "75306546-452b-49b5-b504-186ca914348d",
            "code": "code02",
            "description": "coupoun 02 from api",
            "value": 5,
            "type": 1,
            "type_text": "percentage",
            "start_date": 1619308800,
            "end_date": 1619395200,
            "max_usage": 55,
            "status": "Expired"
        },
        {
            "id": "e6c9fdcf-cc83-49c2-9fad-11127efd5b59",
            "code": "code032",
            "description": "coupoun 02 from api",
            "value": 5,
            "type": 1,
            "type_text": "percentage",
            "start_date": 1619308800,
            "end_date": 1619395200,
            "max_usage": 55,
            "status": "Expired"
        },
        {
            "id": "e913b82a-79da-4917-89b9-5fdfb59038da",
            "code": "coupons01",
            "description": "Coupon 01",
            "value": 10,
            "type": 1,
            "type_text": "percentage",
            "start_date": 1618099200,
            "end_date": 1619827140,
            "max_usage": 100,
            "status": "Active"
        }
    ],
    "meta": {
        "pagination": {
            "total": 4,
            "count": 4,
            "per_page": 10,
            "current_page": 1,
            "total_pages": 1,
            "links": {}
        }
    }
}
```
