# Update a Shipping Zone

Endpoint: `https://api.youcan.shop/shipping-zones/{id}`

Method: `PUT`

## Parameters

| Param Name     | Param Type | Description                 | Required  |
| -------------- | ---------- | ----------------------------| ----------|
| `name`         | string     | shipping zone name          | yes       |
| `display_name` | string     | shipping zone display name  | yes       |
| `countries`    | array,null | shipping zone countries     | no        |
| `is_free`      | boolean    | is free shipping            | no        |
| `is_active`    | boolean    | is shipping zone active     | no         |
| `rate_type`    | string     | (prince, weight)            | no        |
| `rates`        | array      | shipping zone rates         | required if `is_free` false  |
| `rates.*.min`  | float      | shipping rate min           | yes      |
| `rates.*.max`  | float,null | shipping rate max           | no       |
| `rates.*.price`| float      | shipping rate price         | yes      |


## Responses

[200] OK

```json
{
    "message": "Shipping zone updated successfully",
    "http_code": 200,
    "code": "UPDATED",
    "type": "success",
    "data": null
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
