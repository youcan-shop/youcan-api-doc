# Create a menu

Endpoint: `https://api.youcan.shop/menus`

Method: `POST`

## Parameters

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| name | string | Name | yes |
| slug | string | URL slug | yes |
| links |  array of objects [[Link](#link)], null | Array of product ids the upsell will display |
| links.children    |  array of objects [[Link childern](#Links children)], null | Array of product ids the upsell will display |

## Response

[201] Created

```json
{
  "id": "02360486-292e-4bd2-bcae-67b281414c31",
  "name": "Test menu 02",
  "slug": "page-08",
  "is_default": false,
  "links": [
    {
      "id": "5842c635-41f4-40fb-8cdb-5bce1f01549f",
      "name": "Test link 02",
      "link": "/pages/about-us",
      "link_to": 4,
      "link_to_text": "External",
      "order": 1,
      "children": []
    }
  ]
}
```
