# Listing Upsells

Endpoint: `https://api.youcan.shop/upsells` 

Method: `GET`

## Response

[200] Ok

```json
{
    "data": [
        {
            "id": "b28e8479-6787-4f00-aadc-93b233f4af9f",
            "name": "upsell0001",
            "product_offer_ids": [
                "6751f888-57bd-467f-b113-b3f3f556af75"
            ],
            "description": "<p>Buy also this one</p>",
            "footer": "<p>Just buy</p>",
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
        },
        {
            "id": "c4340912-d042-46a7-960c-04510d40d6c8",
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
        },
        {
            "id": "ce80cc44-a6c6-4599-8f62-1500fe20e81c",
            "name": "Test upsel",
            "product_offer_ids": [
                "6751f888-57bd-467f-b113-b3f3f556af75"
            ],
            "description": "<p>Buy also this one pleas</p>",
            "footer": "<p>Please just buy</p>",
            "active": true,
            "weight": "1",
            "actions": {
                "btn_no": {
                    "size": "small",
                    "title": "No",
                    "bg_color": "#FF0000",
                    "font_size": "small",
                    "font_color": "#FFFFFF"
                },
                "btn_yes": {
                    "size": "large",
                    "title": "Yes",
                    "bg_color": "#05BE35",
                    "font_size": "large",
                    "font_color": "#FFFFFF"
                }
            }
        }
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
