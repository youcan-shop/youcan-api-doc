# Listing Categories

Endpoint: `https://api.youcan.shop/categories`

Method: `GET`

## Sorting

- `sort field`:
  - `name`: Category name
  - `created_at`: Category creation date
  - `show_on_collection`: Category visibility in StoreFront

## Searching

To search in categories, add GET param `q`.

`https://api.youcan.shop/categories?q=<SEARCH_VALUE>`

### Searcheable fields

Searchable fields are matched when the field value contains the expression

- `name`
- `slug`
- `description`

## Filters

| Filter Name          | Filter Type | Description                                          |
| -------------------- | ----------- | ---------------------------------------------------- |
| `show_in_collection` | boolean     | get either shown or hidden categories based on value |
| `only_top_level`     | boolean     | when set to true, get only parent categories         |

## Response

[200]

```json
{
  "data": [
    {
      "id": "07cbf517-f3b0-4215-a970-0253af95a7b1",
      "name": "Default category",
      "image": null,
      "slug": "default-category",
      "show_on_collection": false,
      "public_url": "http://my-store.youcan.shop/collections/default-category",
      "description": "This is the default category.",
      "has_parent": false,
      "parent_id": null,
      "is_default": false,
      "images": [],
      "depth": 0,
      "meta": {
        "title": "Default category",
        "description": "This is the default category.",
        "images": [],
        "images_urls": []
      },
      "created_at": "2021-04-12T11:25:00+00:00",
      "updated_at": "2021-04-12T11:25:00+00:00",
      "deleted_at": null,
      "parent": []
    }
    /* ... */
  ],
  "meta": {
    "pagination": {
      "total": 3,
      "count": 3,
      "per_page": 10,
      "current_page": 1,
      "total_pages": 1,
      "links": {}
    }
  }
}
```
