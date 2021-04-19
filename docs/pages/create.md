# Create a page

Endpoint: `https://api.youcan.shop/pages` 

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

[201] Created

```
{
    "id": "676a0db0-0d9a-4022-b681-68cefb1c260a",
    "name": "about-us",
    "slug": "about-us",
    "visibility": "1",
    "public_url": null,
    "content": "<h4>about us</h4>",
    "created_at": "2021-04-19T12:26:46+00:00",
    "meta": {
        "title": "about us",
        "description": "about us description",
        "images": []
    }
}
```
