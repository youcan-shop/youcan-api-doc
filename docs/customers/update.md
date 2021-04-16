# Update a Customer

Endpoint: `https://api.youcan.shop/customers/{id}`

Method: `PUT`

<a name="parameters"></a>

## Parameters

| Param Name     | Param Type | Description                 | Required |
| -------------- | ---------- | ----------------------------| -------- |
| `first_name`   | string     | Customer first name         | no       |
| `last_name`    | string     | Customer last name          | no       |
| `email`        | string     | Customer email              | no       |
| `phone`        | string     | Customer phone number       | no       |
| `country`      | string     | Customer country            | no       |
| `region`       | string     | Customer region             | no       |
| `city`         | string     | Customer city               | no       |
| `notes`        | string     | Customer notes              | no       |

<a name="response"></a>

## Response

[200] OK

```json
{
    "id": "352d2501-5614-44e1-a1e2-c650e7d99f56",
    "first_name": "Mohamed 2",
    "last_name": "AZIZI 2",
    "full_name": "Mohamed 2 AZIZI 2",
    "email": "azizi+customer+2@nextmedia.ma",
    "avatar": "https://www.gravatar.com/avatar/fd340f62c91392a5bc5d939c38a5ef2e?s=100&d=http://api.dotshop.com/store-admin/images/generic_avatar.png",
    "phone": "+212706650841",
    "country": "Morocco",
    "region": "Fes",
    "city": "Meknes",
    "notes": "note 2",
    "location": "Fes, Morocco",
    "created_at": "2021-04-14T23:32:18+00:00",
    "updated_at": "2021-04-15T13:50:39+00:00",
    "deleted_at": null,
    "links": {
        "edit": "http://seller-area.dotshop.com/admin/customers/352d2501-5614-44e1-a1e2-c650e7d99f56/edit"
    },
    "address": [
        {
            "id": "193354a2-5d62-4348-90f9-cb9f1ce40a70",
            "first_name": "mohamed2",
            "last_name": "test2",
            "full_name": "mohamed2 test2",
            "first_line": "Lot ohod 2",
            "second_line": "takkadom 2",
            "company": "nextmedia 2",
            "phone": "+212706650844",
            "country_code": "MA",
            "country_name": "Morocco",
            "state": null,
            "region": "Fes, Meknes",
            "city": "Meknes",
            "zip_code": "50000",
            "default": true,
            "created_at": 1618443138,
            "updated_at": 1618484308
        }
    ]
}
```
