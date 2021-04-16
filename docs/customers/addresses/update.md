# Update an address for a customer

Endpoint: `https://api.youcan.shop/customers/{id}/addresses/{addressId}`

Method: `PUT`

<a name="parameters"></a>

## Parameters

| Param Name     | Param Type | Description                   | Required |
| -------------- | ---------- | ----------------------------- | -------- |
| `first_name`   | string     | Address holder's first name   | no       |
| `last_name`    | string     | Address holder's last name    | no       |
| `company`      | string     | Address holder's company name | no       |
| `phone`        | string     | Address holder's phone number | no       |
| `first_line`   | string     | Address holder's first line   | no       |
| `second_line`  | string     | Address holder's second line  | no       |
| `state`        | string     | Address holder's state        | no       |
| `region`       | string     | Address holder's region       | no       |
| `city`         | string     | Address holder's city         | no       |
| `zip_code`     | string     | Address holder's postal code  | no       |
| `country_code` | string     | Address holder's country code | no       |
| `is_default`   | boolean    | Address holder's country code | no       |

<a name="response"></a>
## Response

[201] Created

```json
{
    "id": "da4d2666-33d2-47de-881b-3dad8c4abf62",
    "first_name": "Hassan",
    "last_name": "AZIZI",
    "full_name": "Hassan AZIZI",
    "email": "azizi+hassan@nextmedia.ma",
    "avatar": "https://www.gravatar.com/avatar/f287649f7dd2d340b5e22704b3622ecd?s=100&d=http://api.dotshop.com/store-admin/images/generic_avatar.png",
    "phone": "+212706650843",
    "country": "Morocco",
    "region": "Fes",
    "city": "Meknes",
    "notes": "note 1",
    "location": "Fes, Morocco",
    "created_at": "2021-04-15T13:55:10+00:00",
    "updated_at": "2021-04-15T13:55:10+00:00",
    "deleted_at": null,
    "links": {
        "edit": "http://seller-area.dotshop.com/admin/customers/da4d2666-33d2-47de-881b-3dad8c4abf62/edit"
    },
    "address": [
        {
            "id": "43cc4816-57dc-4eb1-a828-d2850fe1b42b",
            "first_name": "mohamed",
            "last_name": "AZIZI",
            "full_name": "mohamed AZIZI",
            "first_line": "Lot ohod 2",
            "second_line": "takkadom 2",
            "company": "nextmedia",
            "phone": "+212706650844",
            "country_code": "MA",
            "country_name": "Morocco",
            "state": null,
            "region": "Fes, Meknes",
            "city": "Meknes",
            "zip_code": "50000",
            "default": true,
            "created_at": 1618494926,
            "updated_at": 1618494926
        },
        {
            "id": "d0c40144-c4ed-4af1-91be-9db892608a4f",
            "first_name": "Hassan",
            "last_name": "AZIZI",
            "full_name": "Hassan AZIZI",
            "first_line": "9241 13th Ave SW",
            "second_line": "Floor 54",
            "company": "Google",
            "phone": "+212706650844",
            "country_code": "US",
            "country_name": "United States",
            "state": null,
            "region": "Washington",
            "city": "Seattle",
            "zip_code": "98106",
            "default": false,
            "created_at": 1618494910,
            "updated_at": 1618495221
        }
    ]
}
```
