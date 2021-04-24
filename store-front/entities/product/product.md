Products are an essential part of the ecommerce system, here's a detailed listing of the product entity at YouCan.

| Attribute Name | Type | Description |
| --- | --- | --- |
| id | string | Identifier (UUID) |
| name | string | Product name |
| slug | string | Product SLUG |
| description | string | Product full description |
| price | float | Product price (in store currency) |
| compare_at_price | float,null | Product compare at price (in store currency) |
| track_inventory | bool | Is the product inventory is tracked or not |
| has_variants | bool | Does the product has any variants. If not, we have one `default` variant automatically. |
| [meta](#meta) | JSON | SEO attributes |
| variant_options | array | List of variations for the product |
| created_at | string | Product creation date |

<a name="meta"></a>
## Meta

SEO object to be used for SEO.

| Attribute Name | Type|
| --- | --- |
| title | string |
| description | string |
| images | array |
