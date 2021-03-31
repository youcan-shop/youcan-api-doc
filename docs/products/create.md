# Create a Product

Endpoint: `https://api.youcan.shop/products` 

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
| `vendors` | array\|string[] | List of tags/vendors to assign to product. | no |

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

```
 {
    "id": "dbf8a5a4-4bf9-11ea-ade4-0697b8fb7323",
     "name": "Amazing watch for you",
     "slug": "amazing-smartwatch",
     "public_url": "https://maroc.youcan.shop/products/amazing-smartwatch",
     "thumbnail": "https://cdn.ycan.shop/stores/maroc/products/FyRohvIKye2sbq6MzOf1KAnGiYB1Xt5vRZ7m4xzD_md.jpeg",
     "description": "very long descriiption",
     "price": 100,
     "compare_at_price": 203,
     "cost_price": null,
     "visibility": true,
     "has_variants": true,
     "variants_count": 1,
     "variant_options": [
         {
             "name": "Design",
             "type": 6,
             "values": [
                 "upload-zone"
             ]
         }
     ],
     "inventory": 0,
     "track_inventory": true,
     "you_save_amount": 103,
     "meta": {
         "title": "Amazing smartwatch",
         "description": "Smart Watch, Fitness Tracker with Heart Rate Monitor, Activity Tracker with 1.3\" Touch Screen, IP68 Waterproof Pedometer Smartwatch with Sleep Monitor",
         "images": []
     },
     "created_at": "2020-02-10T11:38:29+00:00",
     "updated_at": "2020-06-02T12:31:35+00:00",
     "deleted_at": false,
     "images": [
         {
             "id": "ca6ee0a7-eb6e-4d75-8f44-bf08cd64258c",
             "name": "stores/maroc/products/FyRohvIKye2sbq6MzOf1KAnGiYB1Xt5vRZ7m4xzD.jpeg",
             "type": 1,
             "url": "https://cdn.ycan.shop/stores/maroc/products/FyRohvIKye2sbq6MzOf1KAnGiYB1Xt5vRZ7m4xzD.jpeg",
             "order": 1,
             "variations": {
                 "original": "https://cdn.ycan.shop/stores/maroc/products/FyRohvIKye2sbq6MzOf1KAnGiYB1Xt5vRZ7m4xzD.jpeg",
                 "sm": "https://cdn.ycan.shop/stores/maroc/products/FyRohvIKye2sbq6MzOf1KAnGiYB1Xt5vRZ7m4xzD_sm.jpeg",
                 "md": "https://cdn.ycan.shop/stores/maroc/products/FyRohvIKye2sbq6MzOf1KAnGiYB1Xt5vRZ7m4xzD_md.jpeg",
                 "lg": "https://cdn.ycan.shop/stores/maroc/products/FyRohvIKye2sbq6MzOf1KAnGiYB1Xt5vRZ7m4xzD_lg.jpeg"
             }
         },
         {
             "id": "e154633a-2784-4366-97ac-7ff561326b4a",
             "name": "stores/maroc/products/M7jAkVcg4QhWD0htcvIT7mWm0Mpo7OqxWSRFaJpv.jpeg",
             "type": 1,
             "url": "https://cdn.ycan.shop/stores/maroc/products/M7jAkVcg4QhWD0htcvIT7mWm0Mpo7OqxWSRFaJpv.jpeg",
             "order": 2,
             "variations": {
                 "original": "https://cdn.ycan.shop/stores/maroc/products/M7jAkVcg4QhWD0htcvIT7mWm0Mpo7OqxWSRFaJpv.jpeg",
                 "sm": "https://cdn.ycan.shop/stores/maroc/products/M7jAkVcg4QhWD0htcvIT7mWm0Mpo7OqxWSRFaJpv_sm.jpeg",
                 "md": "https://cdn.ycan.shop/stores/maroc/products/M7jAkVcg4QhWD0htcvIT7mWm0Mpo7OqxWSRFaJpv_md.jpeg",
                 "lg": "https://cdn.ycan.shop/stores/maroc/products/M7jAkVcg4QhWD0htcvIT7mWm0Mpo7OqxWSRFaJpv_lg.jpeg"
             }
         },
         {
             "id": "814eacc7-72ec-4744-8736-ca38337e31bf",
             "name": "stores/maroc/products/azcMFaHxrsc9rWqPVhNH1bzK06evi0JimoA2Qh51.jpeg",
             "type": 1,
             "url": "https://cdn.ycan.shop/stores/maroc/products/azcMFaHxrsc9rWqPVhNH1bzK06evi0JimoA2Qh51.jpeg",
             "order": 3,
             "variations": {
                 "original": "https://cdn.ycan.shop/stores/maroc/products/azcMFaHxrsc9rWqPVhNH1bzK06evi0JimoA2Qh51.jpeg",
                 "sm": "https://cdn.ycan.shop/stores/maroc/products/azcMFaHxrsc9rWqPVhNH1bzK06evi0JimoA2Qh51_sm.jpeg",
                 "md": "https://cdn.ycan.shop/stores/maroc/products/azcMFaHxrsc9rWqPVhNH1bzK06evi0JimoA2Qh51_md.jpeg",
                 "lg": "https://cdn.ycan.shop/stores/maroc/products/azcMFaHxrsc9rWqPVhNH1bzK06evi0JimoA2Qh51_lg.jpeg"
             }
         }
     ]
 }
```
