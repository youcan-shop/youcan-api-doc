# Get a upsell

Endpoint: `https://api.youcan.shop/upsell/{id}` 

Method: `GET`

## Response

[200] Ok

```
{
    "id": "b28e8479-6787-4f00-aadc-93b233f4af9f",
    "name": "upsell0001",
    "product_offer_ids": [
        "6751f888-57bd-467f-b113-b3f3f556af75"
    ],
    "description": "<p>Buy also this one pleas</p>",
    "footer": "<p>Please just buy</p>",
    "active": false,
    "weight": "1",
    "actions": {
        "btn_no": {
            "size": "small",
            "title": "No",
            "bg_color": "small",
            "font_size": "#FFFFFF",
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
