# Create a page

Endpoint: `https://api.youcan.shop/pages/{id}` 

Method: `POST`

## Parameters

| Param Name     | Param Type | Description                  | Required |
| -------------- | ---------- | -----------------------------| -------- |
| `name`         | string     | Page name                    | yes      |
| `slug`         | string     | Page slug                    | no       |
| `content`      | string     | Page content                 | no       |
| `visibility`   | boolean    | Page visibility              | no       |
| `template`     | string     | Page template                | no       |
| `is_using_page_builder`     | boolean  | Page using page builder  | no    |
| `meta.title`         | string     | Page meta title        | no       |
| `meta.description`   | string     | Page meta description  | no       |

## Response

[200] OK

```
{
    "message": "Page updated successfully",
    "http_code": 200,
    "code": "UPDATED",
    "type": "success",
    "data": null
}
```

[404] Not Found

```json
{
    "status": 404,
    "code": 0,
    "detail": "Page not found",
    "meta": []
}
```
