The Coupon entity at YouCan.

| Attribute Name | Type | Description |
| --- | --- | --- |
| id | string | Identifier (UUID) |
| code | string | Code should be unique in the store |
| description | string | Description |
| value | float | Fixed/Percentage price |
| type |  int (1,0)  | Percentage or fixed |
| start_date | datetime | Start date of the coupon |
| end_date | datetime, null | End date of coupon validity |
| max_usage | int, null | Determine how many times the coupon can be used |
| usage_count | int | Determine how many times the coupon used default is 0 |
| product_ids | int | Represent the products ids the coupon valid for |
| store_id | uuid | Store id |
| created_at | string | Creation date |
| updated_at | string | Updated date |
| deleted_at | string | Deletion date |
