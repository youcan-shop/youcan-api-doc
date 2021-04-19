# Get a Customer

Endpoint: `https://api.youcan.shop/customers/{id}`

Method: `GET`

<a name="response"></a>
## Response

[200] OK

```json
{
    "id": "e579ccdc-9009-43d5-9dfe-6c06bb8dee04",
    "first_name": "Mohamed",
    "last_name": "AZIZI",
    "full_name": "Mohamed AZIZI",
    "email": "azizi+customer+1@nextmedia.ma",
    "avatar": "https://www.gravatar.com/avatar/5e92f1468e5026e85b75875989e53493?s=100&d=http://api.dotshop.com/store-admin/images/generic_avatar.png",
    "phone": "+212706650843",
    "country": "Morocco",
    "region": "Fes",
    "city": "Meknes",
    "notes": "note 1",
    "location": "Fes, Morocco",
    "created_at": "2021-04-15T13:43:11+00:00",
    "updated_at": "2021-04-15T13:43:11+00:00",
    "deleted_at": null,
    "links": {
        "edit": "http://seller-area.dotshop.com/admin/customers/e579ccdc-9009-43d5-9dfe-6c06bb8dee04/edit"
    },
    "address": [
        {
            "id": "d1fb089d-2d09-44f2-8ca7-8ede4eee3c7f",
            "first_name": "mohamed 2",
            "last_name": "testing",
            "full_name": "mohamed 2 testing",
            "first_line": "Lot ohod",
            "second_line": "takkadom",
            "company": "nextmedia",
            "phone": "+212706650843",
            "country_code": "MA",
            "country_name": "Morocco",
            "state": null,
            "region": "Meknes",
            "city": "Meknes",
            "zip_code": "50000",
            "default": true,
            "created_at": 1618494192,
            "updated_at": 1618494192
        }
    ]
}
```
