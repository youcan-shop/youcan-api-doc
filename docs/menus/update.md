# Update a menu

Endpoint: `https://api.youcan.shop/menus/{id}` 

Method: `PUT`

## Parameters

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| name | string | Name | yes |
| slug | string | URL slug | yes |
| links |  array of objects [[Link](#link)], null | Array of links | no
| links.children    |  array of objects [[Link childern](#Links children)], null | Array of links chillers | no

## Response

[200] Ok

```json
{
    "id": "02360486-292e-4bd2-bcae-67b281414c31",
    "name": "Test manue 02 updated",
    "slug": "page-08",
    "is_default": false,
    "links": [
        {
            "id": "5842c635-41f4-40fb-8cdb-5bce1f01549f",
            "name": "Test link 03",
            "link": null,
            "link_to": 4,
            "link_to_text": "External",
            "order": 1,
            "children": []
        }
    ]
}
```
