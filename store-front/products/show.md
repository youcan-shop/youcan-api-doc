# Get product

Endpoint: `https://my-store.com/api/products/{id}` 

Method: `GET`

## Subresources

To include a sub-resource, add GET param `include`.
`https://my-store.com/api/products/{id}?include=<SUBRESOURCE>`

### Available subresources

- `variants`
- `categories`
- `vendors`
- `images`


## Response

[200]

```json
{
  "id": "73f2c86f-e56b-4390-83b2-e94ea3e2c122",
  "name": "Men's Silver Metal Ring",
  "slug": "mens-silver-metal-ring",
  "public_url": "http://my-store.youcan.shop/products/mens-silver-metal-ring",
  "thumbnail": "http://cdn.youcan.shop/stores/my-store/products/xdhlnnFZ0ynHu7XIXSfYQxyj508hBPHGcQO2vxhb_md.jpeg",
  "description": "Lorem ipsum dollor..",
  "price": 86.7,
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
    "title": "Men's Silver Metal Ring",
    "description": "Lorem ipsum dollor..",
    "images": [
      
    ]
  },
  "images": [
    {
      "id": "29aa3524-e3e7-4e19-ae97-594420ad1453",
      "name": "stores/my-store/products/xdhlnnFZ0ynHu7XIXSfYQxyj508hBPHGcQO2vxhb.jpeg",
      "type": 1,
      "url": "http://cdn.youcan.shop/stores/my-store/products/xdhlnnFZ0ynHu7XIXSfYQxyj508hBPHGcQO2vxhb.jpeg",
      "order": 0,
      "variations": {
        "original": "http://cdn.youcan.shop/stores/my-store/products/xdhlnnFZ0ynHu7XIXSfYQxyj508hBPHGcQO2vxhb.jpeg",
        "sm": "http://cdn.youcan.shop/stores/my-store/products/xdhlnnFZ0ynHu7XIXSfYQxyj508hBPHGcQO2vxhb_sm.jpeg",
        "md": "http://cdn.youcan.shop/stores/my-store/products/xdhlnnFZ0ynHu7XIXSfYQxyj508hBPHGcQO2vxhb_md.jpeg",
        "lg": "http://cdn.youcan.shop/stores/my-store/products/xdhlnnFZ0ynHu7XIXSfYQxyj508hBPHGcQO2vxhb_lg.jpeg"
      }
    }
  ]
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
