Shipping Zone entity at YouCan.

| Attribute Name | Type | Description |
| --- | --- | --- |
| id | string | Identifier (UUID) |
| name | string | Shipping zone name |
| display_name | string | shipping zone display name |
| countries | json | shipping zone countries |
| is_free | boolean | is free shipping |
| is_active | boolean | is shipping zone active |
| rate_type | string | shipping zone rate type (price, weight) |

## Shipping Rate
<a name="shipping-rate"></a>

| Attribute Name | Type | Description |
| --- | --- | --- |
| id | string | Identifier (UUID) |
| min | double | minimum shipping rate |
| max | double | maximum shipping rate |
| price | double | shipping rate price |
| shipping_zone_id | string | shipping zone id |
