# Listing Categories

Endpoint: `https://my-store.com/api/categories` 

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
            "id": "8c38330c-9989-477c-a8e9-7f6650526464",
            "name": "The First Ranking",
            "image": "stores/default/categories/EPbYE9k2Pc4H4F9CUdzqHgj9iNxqfp8GwS0uOqtS.png",
            "slug": "category-1",
            "show_on_collection": true,
            "public_url": "http://my-store.youcan.shop/collections/category-1",
            "description": "The first ranking",
            "has_parent": false,
            "parent_id": null,
            "is_default": false,
            "images": {
                "original": "http://cdn.youcan.shop/stores/default/categories/EPbYE9k2Pc4H4F9CUdzqHgj9iNxqfp8GwS0uOqtS.png",
                "sm": "http://cdn.youcan.shop/stores/default/categories/EPbYE9k2Pc4H4F9CUdzqHgj9iNxqfp8GwS0uOqtS_sm.png",
                "md": "http://cdn.youcan.shop/stores/default/categories/EPbYE9k2Pc4H4F9CUdzqHgj9iNxqfp8GwS0uOqtS_md.png",
                "lg": "http://cdn.youcan.shop/stores/default/categories/EPbYE9k2Pc4H4F9CUdzqHgj9iNxqfp8GwS0uOqtS_lg.png"
            },
            "depth": 0,
            "meta": {
                "title": "The First Ranking",
                "description": "The first ranking",
                "images": [],
                "images_urls": []
            },
            "created_at": "2020-11-09T17:24:54+00:00",
            "updated_at": "2020-11-09T17:24:54+00:00",
            "deleted_at": null,
            "parent": []
        },
        {
            "id": "8ef2630e-3c52-4adf-ab1a-d8a8ddfb95fe",
            "name": "The Second Ranking",
            "image": "stores/default/categories/EPbYE9k2Pc4H4F9CUdzqHgj9iNxqfp8GwS0uOqtS.png",
            "slug": "category-2",
            "show_on_collection": true,
            "public_url": "http://my-store.youcan.shop/collections/category-2",
            "description": "The second ranking",
            "has_parent": false,
            "parent_id": null,
            "is_default": false,
            "images": {
                "original": "http://cdn.youcan.shop/stores/default/categories/EPbYE9k2Pc4H4F9CUdzqHgj9iNxqfp8GwS0uOqtS.png",
                "sm": "http://cdn.youcan.shop/stores/default/categories/EPbYE9k2Pc4H4F9CUdzqHgj9iNxqfp8GwS0uOqtS_sm.png",
                "md": "http://cdn.youcan.shop/stores/default/categories/EPbYE9k2Pc4H4F9CUdzqHgj9iNxqfp8GwS0uOqtS_md.png",
                "lg": "http://cdn.youcan.shop/stores/default/categories/EPbYE9k2Pc4H4F9CUdzqHgj9iNxqfp8GwS0uOqtS_lg.png"
            },
            "depth": 0,
            "meta": {
                "title": "The Second Ranking",
                "description": "The second ranking",
                "images": [],
                "images_urls": []
            },
            "created_at": "2020-11-09T17:24:54+00:00",
            "updated_at": "2020-11-09T17:24:54+00:00",
            "deleted_at": null,
            "parent": []
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
