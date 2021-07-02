# Listing Sub categories by category

Endpoint: `https://my-store.com/api/categories/{id}/children` 

Method: `GET`

## Sorting

- `sort_field`:
  - `name`: Category name.
  - `created_at`:  Creation date.

## Response

[200]

```json
{
    "data": [
        {
            "id": "e875783e-07be-4792-952e-6073543d5f48",
            "name": "Modest clothing",
            "image": null,
            "slug": "modest-clothing",
            "show_on_collection": true,
            "public_url": "http://my-store.youcan.shop/collections/modest-clothing",
            "description": null,
            "has_parent": true,
            "parent_id": "636ea8ec-0748-4472-b1a8-402ae52093c8",
            "is_default": false,
            "images": [],
            "depth": 1,
            "meta": {
                "title": "Modest clothing",
                "description": null,
                "images": [],
                "images_urls": []
            },
            "created_at": "2020-11-20T18:37:39+00:00",
            "updated_at": "2020-12-03T17:22:11+00:00",
            "deleted_at": null,
            "parent": {
                "id": "636ea8ec-0748-4472-b1a8-402ae52093c8",
                "name": "Clothing, Shoes & Accessories",
                "image": null,
                "slug": "clothing-shoes-and-accessories",
                "show_on_collection": true,
                "public_url": null,
                "description": null,
                "has_parent": false,
                "parent_id": null,
                "is_default": false,
                "images": [],
                "depth": 0,
                "meta": {
                    "title": "Clothing, Shoes & Accessories",
                    "description": null,
                    "images": [],
                    "images_urls": []
                },
                "created_at": "2020-11-20T18:36:52+00:00",
                "updated_at": "2020-11-20T18:36:52+00:00",
                "deleted_at": null
            }
        },
        {
            "id": "2a5870e0-b893-4768-a422-118e531898c8",
            "name": "Women's Clothing",
            "image": null,
            "slug": "womens-clothing",
            "show_on_collection": true,
            "public_url": "http://my-store.youcan.shop/collections/womens-clothing",
            "description": null,
            "has_parent": true,
            "parent_id": "636ea8ec-0748-4472-b1a8-402ae52093c8",
            "is_default": false,
            "images": [],
            "depth": 1,
            "meta": {
                "title": "Women's Clothing",
                "description": null,
                "images": [],
                "images_urls": []
            },
            "created_at": "2020-11-20T18:37:13+00:00",
            "updated_at": "2020-12-03T17:21:04+00:00",
            "deleted_at": null
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

