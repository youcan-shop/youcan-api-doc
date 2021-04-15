# Update a Upsell

Endpoint: `https://api.youcan.shop/upsells/{id}` 

Method: `PUT`

## Parameters

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| name | string | Name | yes
| description | string, null | Description | no
| product_id | uuid | Product id concerned by this upsell | yes
| product_offer_ids |  array | Array of product ids the upsell will display | yes
| actions | array of objects [[Action](../entities/upsells/upsell.md)] | Yes, No buttons with their setting | yes
| footer | string, null | Text displayed in bottom for upsell | no

## Response

[200] Ok

```
{
    "id": "b28e8479-6787-4f00-aadc-93b233f4af9f",
    "name": "upsell0001updated",
    "product_offer_ids": [
        "6751f888-57bd-467f-b113-b3f3f556af75"
    ],
    "description": "<p>Buy also this one </p>",
    "footer": "<p>Limited offer</p>",
    "active": false,
    "weight": "1",
    "actions": {
        "btn_no": {
            "size": "small",
            "title": "No",
            "bg_color": "#FFFFFF",
            "font_size": "small",
            "font_color": "#FF0000"
        },
        "btn_yes": {
            "size": "large",
            "title": "Yes",
            "bg_color": "#FFFFFF",
            "font_size": "large",
            "font_color": "#05BE35"
        }
    }
}
```
