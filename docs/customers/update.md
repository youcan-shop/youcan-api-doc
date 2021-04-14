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

<a name="reponse"></a>
## Response

[200] OK

```json
{
    "id": "0d3739eb-2129-47a6-a770-4703ed49c881",
    "first_name": "Update",
    "last_name": "Update",
    "full_name": "Update Update",
    "email": "azizi+update@nextmedia.ma",
    "avatar": "https://www.gravatar.com/avatar/f0cf72fafc33a08c47fc5f4e5511e6f9?s=100&d=http://api.dotshop.com/store-admin/images/generic_avatar.png",
    "phone": "7728160",
    "country": "France",
    "region": "Fes",
    "city": "Fes",
    "notes": "Note update",
    "location": "Fes, France",
    "created_at": "2021-04-13T17:36:17+00:00",
    "updated_at": "2021-04-14T12:07:22+00:00",
    "deleted_at": null,
    "links": {
        "edit": "http://seller-area.dotshop.com/admin/customers/0d3739eb-2129-47a6-a770-4703ed49c881/edit"
    }
}
```
