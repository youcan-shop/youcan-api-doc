# Increment a product inventory

Endpoint: `https://api.youcan.shop/products/{id}/inventory/increment` 

Method: `PUT`

## Parameters

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| `varaint_id` | string | Product variant id | yes |
| `inventory` | int | Product stock | yes |


## Response

[200] Updated

```json
{
    "id": "f7ae7509-1fc4-44f7-9241-ca6aa1e3f89f",
    "variations": {
        "color": "Red"
    },
    "options": [
        "color"
    ],
    "values": [
        "Red"
    ],
    "price": 10,
    "compare_at_price": 15,
    "weight": null,
    "sku": null,
    "barcode": null,
    "inventory": 66,
    "is_selected": false,
    "is_default": false,
    "image": {
        "name": "stores/7b7f84b5d55410cf87bbffc9317b1546/products/dMKxUVDjn3iPxZ0IGbDR32rnP2SvmCUj5Th6Pvxo.jpeg",
        "url": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/dMKxUVDjn3iPxZ0IGbDR32rnP2SvmCUj5Th6Pvxo.jpeg"
    },
    "created_at": "2021-04-07T13:52:33+00:00",
    "updated_at": "2021-04-15T14:58:38+00:00",
    "product": {
        "id": "ea56bdd1-8ad0-4c6b-b708-3f4c331d1678",
        "name": "OPPO A1K",
        "slug": "oppo-a1k",
        "public_url": null,
        "thumbnail": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/O0UmVapEcd5AzEdI5n7MesKQPrEsRZkjBONDIxdr_md.jpeg",
        "description": "<p>OPPO A1K</p>",
        "price": 10,
        "compare_at_price": 15,
        "cost_price": null,
        "visibility": true,
        "has_variants": true,
        "variants_count": 2,
        "variant_options": [
            {
                "name": "color",
                "type": 3,
                "values": [
                    {
                        "value": "Red",
                        "preview": "#D0021B"
                    },
                    {
                        "value": "Black",
                        "preview": "#000000"
                    }
                ]
            }
        ],
        "inventory": 151,
        "track_inventory": true,
        "meta": {
            "title": "OPPO A1K",
            "description": "OPPO A1K",
            "images": [
                {
                    "path": "stores/7b7f84b5d55410cf87bbffc9317b1546/products/ZGXIvIpT2166N37xR81oPfBvUoWAN5WFi9nGVXb7.png",
                    "link": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/ZGXIvIpT2166N37xR81oPfBvUoWAN5WFi9nGVXb7.png"
                }
            ]
        },
        "advanced_options": {
            "enabled": false,
            "related_products": []
        },
        "created_at": "2021-04-02T15:39:55+00:00",
        "updated_at": "2021-04-15T13:36:40+00:00",
        "deleted_at": false,
        "images": [
            {
                "id": "8c52bba1-fea1-42b1-ab92-1e7107c78954",
                "name": "stores/7b7f84b5d55410cf87bbffc9317b1546/products/O0UmVapEcd5AzEdI5n7MesKQPrEsRZkjBONDIxdr.jpeg",
                "type": 1,
                "url": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/O0UmVapEcd5AzEdI5n7MesKQPrEsRZkjBONDIxdr.jpeg",
                "order": 2,
                "variations": {
                    "original": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/O0UmVapEcd5AzEdI5n7MesKQPrEsRZkjBONDIxdr.jpeg",
                    "sm": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/O0UmVapEcd5AzEdI5n7MesKQPrEsRZkjBONDIxdr_sm.jpeg",
                    "md": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/O0UmVapEcd5AzEdI5n7MesKQPrEsRZkjBONDIxdr_md.jpeg",
                    "lg": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/O0UmVapEcd5AzEdI5n7MesKQPrEsRZkjBONDIxdr_lg.jpeg"
                }
            },
            {
                "id": "071f1f4e-51ae-496d-98b3-b366480cedb1",
                "name": "stores/7b7f84b5d55410cf87bbffc9317b1546/products/bkiMkJm7XUVAGWleVyEP6l11aIz1lqnX4EO4lRPW.jpeg",
                "type": 1,
                "url": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/bkiMkJm7XUVAGWleVyEP6l11aIz1lqnX4EO4lRPW.jpeg",
                "order": 4,
                "variations": {
                    "original": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/bkiMkJm7XUVAGWleVyEP6l11aIz1lqnX4EO4lRPW.jpeg",
                    "sm": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/bkiMkJm7XUVAGWleVyEP6l11aIz1lqnX4EO4lRPW_sm.jpeg",
                    "md": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/bkiMkJm7XUVAGWleVyEP6l11aIz1lqnX4EO4lRPW_md.jpeg",
                    "lg": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/bkiMkJm7XUVAGWleVyEP6l11aIz1lqnX4EO4lRPW_lg.jpeg"
                }
            },
            {
                "id": "b78a36da-2178-47ef-bf6f-26335176953b",
                "name": "stores/7b7f84b5d55410cf87bbffc9317b1546/products/dMKxUVDjn3iPxZ0IGbDR32rnP2SvmCUj5Th6Pvxo.jpeg",
                "type": 1,
                "url": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/dMKxUVDjn3iPxZ0IGbDR32rnP2SvmCUj5Th6Pvxo.jpeg",
                "order": 4,
                "variations": {
                    "original": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/dMKxUVDjn3iPxZ0IGbDR32rnP2SvmCUj5Th6Pvxo.jpeg",
                    "sm": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/dMKxUVDjn3iPxZ0IGbDR32rnP2SvmCUj5Th6Pvxo_sm.jpeg",
                    "md": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/dMKxUVDjn3iPxZ0IGbDR32rnP2SvmCUj5Th6Pvxo_md.jpeg",
                    "lg": "http://cdn.youcan.shop/stores/7b7f84b5d55410cf87bbffc9317b1546/products/dMKxUVDjn3iPxZ0IGbDR32rnP2SvmCUj5Th6Pvxo_lg.jpeg"
                }
            }
        ]
    }
}
```
