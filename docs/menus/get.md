# Get a menu

Endpoint: `https://api.youcan.shop/menus/{id}` 

Method: `GET`

## Response

[200] Ok

```json
{
    "id": "18d696bd-53ed-4781-ae0e-fa30673542c0",
    "name": "Acerca de la tienda",
    "slug": "footer-about",
    "is_default": false,
    "links": [
        {
            "id": "888ce555-b618-4fdf-a921-2ca0fd8b69db",
            "name": "Acerca de nosotros",
            "link": "/pages/about-us",
            "link_to": 4,
            "link_to_text": "External",
            "order": 0,
            "children": []
        },
        {
            "id": "a521b745-2517-4205-9c4d-57b05f894682",
            "name": "Cómo pagar",
            "link": "/pages/how-to-pay",
            "link_to": 4,
            "link_to_text": "External",
            "order": 1,
            "children": []
        },
        {
            "id": "a2ba7b79-352c-4e52-ba37-9a7aa1e3133d",
            "name": "Envío y Entrega",
            "link": "/pages/shipping-delivery",
            "link_to": 4,
            "link_to_text": "External",
            "order": 2,
            "children": []
        }
    ]
}
```
