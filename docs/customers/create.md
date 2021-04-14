# Create a Customer

Endpoint: `https://api.youcan.shop/customers`

Method: `POST`

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

<a name="reponse"></a>
## Response

[201] Created

```json
{
    "id": "834deefd-a45a-4636-96a2-6f69f9082fad",
    "first_name": "Mohamed",
    "last_name": "AZIZI",
    "full_name": "Mohamed AZIZI",
    "email": "azizi+customer@nextmedia.ma",
    "avatar": "https://www.gravatar.com/avatar/b3e87b218e00952a2db24bc608c1eb1b?s=100&d=http://api.dotshop.com/store-admin/images/generic_avatar.png",
    "phone": "77281652",
    "country": "Maroc",
    "region": "Meknes",
    "city": "Meknes",
    "notes": "Note",
    "location": "Meknes, Maroc",
    "created_at": "2021-04-14T12:02:27+00:00",
    "updated_at": "2021-04-14T12:02:27+00:00",
    "deleted_at": null,
    "links": {
        "edit": "http://seller-area.dotshop.com/admin/customers/834deefd-a45a-4636-96a2-6f69f9082fad/edit"
    }
}
```
