# Listing Products

Endpoint: `https://my-store.com/api/categories/{id}/products` 

Method: `GET`

## Sorting

- `sort_field`:
  - `name`: Product name.
  - `price`: Product price.
  - `you_save_amount`: The different between price and compare at price.
  - `created_at`:  Creation date.

## Response

[200]

```json
{
    "data": [
        {
            "id": "44d71b37-7d1d-4fc0-a69d-72b3b66352bd",
            "name": "Silver Rhodium Wedding Ring",
            "slug": "silver-rhodium-wedding-ring",
            "public_url": null,
            "thumbnail": "http://cdn.youcan.shop/stores/my-store/products/gnuYpd98X6huXaR51aL8GO23IYnERB08KUMOhdLA_md.jpeg",
            "description": "Lorem ipsum dollor..",
            "price": 27.54,
            "compare_at_price": null,
            "has_variants": true,
            "variants_count": 22,
            "variant_options": [
                {
                    "name": "Size",
                    "type": 2,
                    "values": [
                        "9",
                        "10",
                        "11",
                        "12"
                    ]
                }
            ],
            "track_inventory": true,
            "meta": {
                "title": "Silver Rhodium Wedding Ring",
                "description": "Lorem ipsum dollor..",
                "images": []
            },
            "images": [
                {
                    "id": "14cc6217-0d8e-4f6e-b746-7e8f1736747f",
                    "name": "stores/my-store/products/gnuYpd98X6huXaR51aL8GO23IYnERB08KUMOhdLA.jpeg",
                    "type": 1,
                    "url": "http://cdn.youcan.shop/stores/my-store/products/gnuYpd98X6huXaR51aL8GO23IYnERB08KUMOhdLA.jpeg",
                    "order": 1,
                    "variations": {
                        "original": "http://cdn.youcan.shop/stores/my-store/products/gnuYpd98X6huXaR51aL8GO23IYnERB08KUMOhdLA.jpeg",
                        "sm": "http://cdn.youcan.shop/stores/my-store/products/gnuYpd98X6huXaR51aL8GO23IYnERB08KUMOhdLA_sm.jpeg",
                        "md": "http://cdn.youcan.shop/stores/my-store/products/gnuYpd98X6huXaR51aL8GO23IYnERB08KUMOhdLA_md.jpeg",
                        "lg": "http://cdn.youcan.shop/stores/my-store/products/gnuYpd98X6huXaR51aL8GO23IYnERB08KUMOhdLA_lg.jpeg"
                    }
                }
            ]
        },
        {
            "id": "c26be441-6de5-4ed0-9362-7f9e479f00d1",
            "name": "Men's Silver Blue Ebony Ring",
            "slug": "mens-silver-blue-ebony-ring",
            "public_url": null,
            "thumbnail": "http://cdn.youcan.shop/stores/my-store/products/sp3LiNOCQTQilYKOU1SFvOLdG1CB1hQDFhy4qsoh_md.jpeg",
            "description": "Lorem ipsum dollor..",
            "price": 84.46,
            "compare_at_price": null,
            "has_variants": true,
            "variants_count": 15,
            "variant_options": [
                {
                    "name": "Size",
                    "type": 2,
                    "values": [
                        "18",
                        "19",
                        "20"
                    ]
                }
            ],
            "track_inventory": true,
            "meta": {
                "title": "Men's Silver Blue Ebony Ring",
                "description": "Lorem ipsum dollor..",
                "images": []
            },
            "images": [
                {
                    "id": "b7bc9ea3-4251-43b6-8dcf-02c5e4158804",
                    "name": "stores/my-store/products/sp3LiNOCQTQilYKOU1SFvOLdG1CB1hQDFhy4qsoh.jpeg",
                    "type": 1,
                    "url": "http://cdn.youcan.shop/stores/my-store/products/sp3LiNOCQTQilYKOU1SFvOLdG1CB1hQDFhy4qsoh.jpeg",
                    "order": 1,
                    "variations": {
                        "original": "http://cdn.youcan.shop/stores/my-store/products/sp3LiNOCQTQilYKOU1SFvOLdG1CB1hQDFhy4qsoh.jpeg",
                        "sm": "http://cdn.youcan.shop/stores/my-store/products/sp3LiNOCQTQilYKOU1SFvOLdG1CB1hQDFhy4qsoh_sm.jpeg",
                        "md": "http://cdn.youcan.shop/stores/my-store/products/sp3LiNOCQTQilYKOU1SFvOLdG1CB1hQDFhy4qsoh_md.jpeg",
                        "lg": "http://cdn.youcan.shop/stores/my-store/products/sp3LiNOCQTQilYKOU1SFvOLdG1CB1hQDFhy4qsoh_lg.jpeg"
                    }
                }
            ]
        }
    ],
    "meta": {
        "pagination": {
            "total": 2,
            "count": 2,
            "per_page": 10,
            "current_page": 1,
            "total_pages": 1,
            "links": {}
        }
    }
}
```

[404]

```json
{
    "status": 404,
    "code": 404,
    "detail": "category not found",
    "meta": []
}
```

