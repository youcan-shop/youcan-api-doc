# Listing Products

Endpoint: `https://my-store.com/api/products` 

Method: `GET`

## Sorting

- `sort_field`:
  - `name`: Product name.
  - `price`: Product price.
  - `you_save_amount`: The different between price and compare at price.
  - `created_at`:  Creation date.

## Subresources

To include a sub-resource, add GET param `include`.
`https://my-store.com/api/products?include=<SUBRESOURCE>`

### Available subresources

- `variants`
- `categories`
- `vendors`
- `images`

## Response

[200]

```json
{
    "data": [
        {
            "id": "1d7e9ec3-77e5-4bb2-bffd-d36b97b1dfa3",
            "name": "Second product",
            "slug": "product-2",
            "public_url": "http://my-store.youcan.shop/products/product-2",
            "thumbnail": "http://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr_md.png",
            "description": "<p>The second product</p>",
            "price": 200,
            "compare_at_price": 250,
            "has_variants": false,
            "variants_count": 1,
            "variant_options": [],
            "track_inventory": false,
            "meta": {
                "title": "Second product",
                "description": "The second product",
                "images": [
                    {
                        "path": "stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr.png",
                        "link": "http://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr.png"
                    }
                ]
            },
            "images": [
                {
                    "id": "6d626432-3246-4202-93c6-afbf5b974dc8",
                    "name": "stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr.png",
                    "type": 1,
                    "url": "http://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr.png",
                    "order": 1,
                    "variations": {
                        "original": "http://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr.png",
                        "sm": "http://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr_sm.png",
                        "md": "http://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr_md.png",
                        "lg": "http://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr_lg.png"
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
                "next": "https://my-store.com/api/products?page=2"
            }
        }
    }
}
```
