# Login a customer

Endpoint: `https://my-store.youcan.shop/api/customers/orders`

Method: `GET`

To authenticate you get the customer token for the [Login endpoint](/store-front/customers/login) 

[401] Unauthorized
```json
{
    "status": 401,
    "detail": "Unauthenticated.",
    "meta": []
}
```

[200] OK
```json
{
    "data": [
        {
            "id": "12d23b0b-2efd-44c5-af88-360e144147bb",
            "ref": "062",
            "vat": 0,
            "total": 10,
            "notes": "\n172.18.0.7\n\n",
            "status": 1,
            "tags": [],
            "extra_fields": null,
            "is_refunded_by_platform": false,
            "platform_fee": 0,
            "created_at": "2021-04-28T14:19:05+00:00",
            "updated_at": "2021-04-28T14:19:05+00:00",
            "links": {
                "self": "http://seller-area.youcan.shop/admin/orders/12d23b0b-2efd-44c5-af88-360e144147bb",
                "edit": "http://seller-area.youcan.shop/admin/orders/12d23b0b-2efd-44c5-af88-360e144147bb/edit"
            },
            "payment": {
                "status_text": "pending",
                "status": 5,
                "created_at": "2021-04-28 14:19",
                "updated_at": "2021-04-28 14:19",
                "payload": {
                    "gateway": "cod",
                    "gateway_id": "5816ebe1-2c7f-4442-a467-4a34bc844fd1",
                    "thank-you-message": "شكرا على طلبك!",
                    "note": null
                },
                "address": []
            },
            "shipping": {
                "status_text": "unfulfilled",
                "status": 2,
                "price": 0,
                "is_free": true,
                "tracking_number": null,
                "payload": {
                    "id": "05c6d910-9469-4407-b966-ca0869b24c08",
                    "compound_id": "sz_05c6d910-9469-4407-b966-ca0869b24c08",
                    "instance_class_name": "YouCan\\Common\\Entities\\ShippingZone",
                    "name": "Fast Shipping Worldwide",
                    "display_name": "Fast Shipping Worldwide",
                    "price": 0,
                    "is_free": true,
                    "is_active": true
                },
                "created_at": "2021-04-28 14:19",
                "updated_at": "2021-04-28 14:19",
                "address": []
            },
            "refunds": [],
            "variants": [
                {
                    "id": "dc00d6bc-5eed-4eca-93e8-f711b4892972",
                    "price": 10,
                    "quantity": 1,
                    "created_at": 1619619545,
                    "updated_at": 1619619545,
                    "extra_fields": [],
                    "variant": {
                        "id": "487eff9a-97c2-43cb-8806-a8f7a1966ea4",
                        "variations": {
                            "default": "default"
                        },
                        "options": [
                            "default"
                        ],
                        "values": [
                            "default"
                        ],
                        "price": 10,
                        "compare_at_price": 15,
                        "weight": 0,
                        "sku": null,
                        "barcode": null,
                        "inventory": 1,
                        "is_selected": false,
                        "is_default": false,
                        "image": {
                            "name": null,
                            "url": null
                        },
                        "created_at": "2021-04-07T17:22:14+00:00",
                        "updated_at": "2021-04-22T11:07:35+00:00",
                        "product": {
                            "id": "6a8f1c4e-1d11-4cc7-bd44-db33355f6279",
                            "name": "المنتج الأول",
                            "slug": "product-1",
                            "public_url": null,
                            "thumbnail": "http://cdn.youcan.shop/stores/default/products/66SEhP6ZCMJArbIHVT5XgkQOEU6q077C4TIfQMk4_md.png",
                            "description": "<p>المنتج الأول</p>",
                            "price": 10,
                            "compare_at_price": 15,
                            "cost_price": null,
                            "visibility": true,
                            "has_variants": false,
                            "variants_count": 1,
                            "variant_options": [],
                            "inventory": 1,
                            "track_inventory": true,
                            "meta": {
                                "title": "المنتج الأول",
                                "description": "المنتج الأول",
                                "images": [
                                    {
                                        "path": "stores/default/products/66SEhP6ZCMJArbIHVT5XgkQOEU6q077C4TIfQMk4.png",
                                        "link": "http://cdn.youcan.shop/stores/default/products/66SEhP6ZCMJArbIHVT5XgkQOEU6q077C4TIfQMk4.png"
                                    }
                                ]
                            },
                            "advanced_options": {
                                "enabled": false,
                                "related_products": []
                            },
                            "created_at": "2021-04-07T17:22:14+00:00",
                            "updated_at": "2021-04-22T11:07:42+00:00",
                            "deleted_at": false,
                            "images": [
                                {
                                    "id": "7796f12e-c5b0-4444-9f7d-806f686c2056",
                                    "name": "stores/default/products/66SEhP6ZCMJArbIHVT5XgkQOEU6q077C4TIfQMk4.png",
                                    "type": 1,
                                    "url": "http://cdn.youcan.shop/stores/default/products/66SEhP6ZCMJArbIHVT5XgkQOEU6q077C4TIfQMk4.png",
                                    "order": 1,
                                    "variations": {
                                        "original": "http://cdn.youcan.shop/stores/default/products/66SEhP6ZCMJArbIHVT5XgkQOEU6q077C4TIfQMk4.png",
                                        "sm": "http://cdn.youcan.shop/stores/default/products/66SEhP6ZCMJArbIHVT5XgkQOEU6q077C4TIfQMk4_sm.png",
                                        "md": "http://cdn.youcan.shop/stores/default/products/66SEhP6ZCMJArbIHVT5XgkQOEU6q077C4TIfQMk4_md.png",
                                        "lg": "http://cdn.youcan.shop/stores/default/products/66SEhP6ZCMJArbIHVT5XgkQOEU6q077C4TIfQMk4_lg.png"
                                    }
                                }
                            ]
                        }
                    }
                }
            ]
        }
    ],
    "meta": {
        "pagination": {
            "total": 1,
            "count": 1,
            "per_page": 10,
            "current_page": 1,
            "total_pages": 1,
            "links": {}
        }
    }
}
```
