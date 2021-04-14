# Create a Coupon

Endpoint: `https://api.youcan.shop/coupons` 

Method: `POST`

## Parameters

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| `code` | string | Code in alpha numeric | yes |
| `description` | string | Description | yes |
| `value` | float | Coupon value in fixed price or percentage | yes |
| `type` | int | Value type 1: percentage, 2: Fixed | yes |
| `start_date` | Datetime | Start date of coupon validity | yes |
| `end_date` | Datetime | End date of coupon validity | no |
| `max_usage` | int | How many times the coupon can be used | no |
| `product_ids` | string[] | List of product IDs the coupon is valid for | no |

## Response

[201] Created

```
 {
    "id": "5913f1f7-f14d-4046-8a7d-701ab8189f11",
    "code": "code0332",
    "description": "coupoun 02 from api",
    "value": 5,
    "type": 1,
    "type_text": "percentage",
    "start_date": 1619308800,
    "end_date": 1619395200,
    "max_usage": 55,
    "status": "Expired"
}
```
