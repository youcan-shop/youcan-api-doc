# Update a Coupon

Endpoint: `https://api.youcan.shop/coupons/{id}` 

Method: `PUT`

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
| `product_ids` | string[] | List of product IDs the coupon is valid for | yes |

## Response

[200] Ok

```json
{
    "id": "2e62a766-af79-49b1-b57b-0a2fdbaeec65",
    "code": "code03323",
    "description": "coupoun 02 from api updated",
    "value": 5,
    "type": 1,
    "type_text": "percentage",
    "start_date": 1619308800,
    "end_date": 1619395200,
    "max_usage": 55,
    "status": "Expired"
}
```
