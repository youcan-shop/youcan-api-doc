# Update a Category

Endpoint: `https://api.youcan.shop/categories/{id}`

Method: `PUT`

## Parameters

| Param Name           | Param Type    | Description           | Required |
| -------------------- | ------------- | --------------------- | -------- |
| `name`               | string        | Category name         | yes      |
| `slug`               | string        | Category slug         | yes      |
| `description`        | string        | Category description  | no       |
| `image`              | File          | Category image        | no       |
| `parent_id`          | uuid          | Categorie's parent id | no       |
| `show_on_collection` | boolean       | Category visibility   | no       |
| `meta`      | [Meta](/store-admin/categories/create#meta) | Category metadata     | no       |

## Response

[422] Unprocessable Entity

```json
// Returned when category's parent is a child category
{
  "status": 422,
  "code": "",
  "detail": "The parent category is not a top level category",
  "meta": []
}
```

[201] Created

```json
{
  "id": "dc20f000-cea4-4205-86be-dbec477bd958",
  "name": "test API",
  "image": "stores/d5feb68cb828b2f4ffee99ad61cf71cf/category/D8xnACeovM30k088bU2M6YDovXsKiq67ckwBaC58.png",
  "slug": "test-aypiay",
  "show_on_collection": false,
  "public_url": null,
  "description": "this is a description",
  "has_parent": false,
  "parent_id": null,
  "is_default": false,
  "images": [],
  "depth": 0,
  "meta": {
    "title": "test API",
    "description": "this is a description",
    "images": [
      "stores/d5feb68cb828b2f4ffee99ad61cf71cf/category/CWn50KJRDEZ7VLqURlt0YajLw4ZmLfsROajePbPO.png",
      "stores/d5feb68cb828b2f4ffee99ad61cf71cf/category/me1dvG3MiVOgMBlb1vt7tkrzdb8gAk9oq47NIasZ.png"
    ],
    "images_urls": []
  },
  "created_at": "2021-04-13T18:09:57+00:00",
  "updated_at": "2021-04-13T18:09:57+00:00",
  "deleted_at": null,
  "parent": []
}
```