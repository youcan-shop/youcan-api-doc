# Decrement a product inventory

Endpoint: `https://api.youcan.shop/products/{id}/inventory/decrement` 

Method: `PUT`

## Parameters

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| `varaint_id` | string | Product variant id | yes |
| `inventory` | int | Product stock | yes |


## Response

[200] Updated

```
{
    "message": "The resource has been successfully decremented.",
    "http_code": 200,
    "code": "UPDATED",
    "type": "success",
    "data": {
        "product_inventory": 55,
        "variant_inventory": 40
    }
}
```
