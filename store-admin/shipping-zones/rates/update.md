# Update a Shipping Rate

Endpoint: `https://api.youcan.shop/shipping-zones/{id}/rates`

Method: `PUT`

<a name="parameters"></a>

## Parameters

## ShippingRate

| Param Name     | Param Type | Description                   | Required |
| -------------- | ---------- | ----------------------------- | -------- |
| `rates`        | array      | shipping zone rates           | no   |
| `rates.*.min`  | float      | shipping rate min             | yes      |
| `rates.*.max`  | float,null | shipping rate max             | no       |
| `rates.*.price`| float      | shipping rate price           | yes      |


<a name="response"></a>
## Response

[200] OK

```json
{
    "message": "Shipping rate updated successfully",
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
