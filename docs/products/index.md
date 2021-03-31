# Listing Products

Endpoint: `https://api.youcan.shop/products` 

Method: `GET`

## Sorting

- `sort_field`:
  - `name`: Product name.
  - `price`: Product price.
  - `orders_count`: Product orders count.
  - `you_save_amount`: The different between price and compare at price.

## Filters

| Field Name | Operator | Value type | Description |
| --- | --- | --- | --- |
| `inventory` | `<`, `<`, `=` | number | Product inventory |
| `trashed` | `=` | bool | Include deleted products |


## Response

[200]

```json
{
    "data": [
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
        },
        /* ... */
    ],
    "meta": {
        "pagination": {
            "total": 21,
            "count": 10,
            "per_page": 10,
            "current_page": 1,
            "total_pages": 3,
            "links": {
                "next": "https://seller-area.youcan.shop/admin/api/products?page=2"
            }
        }
    }
}
```
