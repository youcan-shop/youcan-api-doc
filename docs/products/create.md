# Create a Product

Endpoint: `https://seller-area.youcan.shop/admin/api/products` 

Method: `POST`

## Parameters

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| `name` | string | Product name | yes |
| `description` | string | Product description | no |
| `visibility` | bool | Is product visible for customers | no |
| `track_inventory` | bool | Should the inventory be tracked? | no |
| `inventory` | int | Product stock | no |
| `has_variants` | bool | Product contain variants? | yes |
| `price` | float | Product price | yes |
| `compare_at_price` | float | Product compare price | no |
| `cost_price` | float | Product cost price | no |
| `variant_options` | array | List of product [variant options](#variant_options). | no |
| `categories` | string[] | List of categories IDs to attach to product | no |
| `variants` | array | List of product [variants](#variants). | no |

<a name="variant_options"></a>
### Variant Options

Ex: `[{"name": "Size", "type": 4, "values": ["M", "L"]}]`

<a name="variants"></a>
### Variants

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| `variations` | object | Key, value pair of select variation. Ex: `{"Color": "Red", "Size": "M"}` | yes |
| `price` | float | Variant price. Default to product price. | no |
| `weight` | float | Variant weight. | no |
| `sku` | string | Variant SKU. | no |
| `barcode` | string | Variant barcode. | no |
| `inventory` | int | Variant inventory. | no |
| `image` | string | Variant image path if any. | no |

## Response

[201] Created
