# Listing Customers

Endpoint: `https://api.youcan.shop/customers`

Method: `GET`

## Searching

To search in customers, add GET param `q`.
`https://seller-area.youcan.shop/admin/api/customers?q=<SEARCH_VALUE>`

### Searcheable fields

Searchable fields are matched when the field value contains the expression

- `Customer first name`
- `Customer last name`
- `Customer phone`
- `Customer email`

## Response

[200]

```json
{
    "data": [
        {
            "id": "6d4cb5cd-6e0a-49cf-934d-6c63eeaf41f2",
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
            "created_at": "2021-04-13T17:38:27+00:00",
            "updated_at": "2021-04-13T17:38:27+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/6d4cb5cd-6e0a-49cf-934d-6c63eeaf41f2/edit"
            }
        },
        {
            "id": "de9f099d-1a14-491d-8a1b-6457c71c9315",
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
            "created_at": "2021-04-13T17:38:00+00:00",
            "updated_at": "2021-04-13T17:38:00+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/de9f099d-1a14-491d-8a1b-6457c71c9315/edit"
            }
        },
        {
            "id": "c9bcaf7a-be1c-43bc-a051-b582ef72063c",
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
            "created_at": "2021-04-13T17:37:38+00:00",
            "updated_at": "2021-04-13T17:37:38+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/c9bcaf7a-be1c-43bc-a051-b582ef72063c/edit"
            }
        },
        {
            "id": "c80887b6-1d65-4b16-bf1a-3929df7a8fe2",
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
            "created_at": "2021-04-13T17:36:32+00:00",
            "updated_at": "2021-04-13T17:36:32+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/c80887b6-1d65-4b16-bf1a-3929df7a8fe2/edit"
            }
        },
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
            "updated_at": "2021-04-14T11:29:35+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/0d3739eb-2129-47a6-a770-4703ed49c881/edit"
            }
        },
        {
            "id": "0dd4cca1-6d4c-43f5-83c9-a8107faa82cf",
            "first_name": "Mohamed",
            "last_name": "azizi",
            "full_name": "Mohamed azizi",
            "email": null,
            "avatar": "https://www.gravatar.com/avatar/d41d8cd98f00b204e9800998ecf8427e?s=100&d=http://api.dotshop.com/store-admin/images/generic_avatar.png",
            "phone": "77261542",
            "country": "France",
            "region": "ok",
            "city": "Meknes",
            "notes": "",
            "location": "Ra's al Khaymah, France",
            "created_at": "2021-04-08T13:08:47+00:00",
            "updated_at": "2021-04-08T13:08:48+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/0dd4cca1-6d4c-43f5-83c9-a8107faa82cf/edit"
            }
        },
        {
            "id": "06559c47-348e-486f-ada0-186171f94f2e",
            "first_name": "محمد",
            "last_name": "عزيزي",
            "full_name": "محمد عزيزي",
            "email": null,
            "avatar": "https://www.gravatar.com/avatar/d41d8cd98f00b204e9800998ecf8427e?s=100&d=http://api.dotshop.com/store-admin/images/generic_avatar.png",
            "phone": "77261542",
            "country": "imo",
            "region": "a",
            "city": "Meknes",
            "notes": "",
            "location": "Saint Paul, imo",
            "created_at": "2021-04-08T13:01:06+00:00",
            "updated_at": "2021-04-08T13:01:51+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/06559c47-348e-486f-ada0-186171f94f2e/edit"
            }
        },
        {
            "id": "d2cbe1dd-52dc-485a-8eb5-9aac08fe485e",
            "first_name": "Ahmed",
            "last_name": "Boo",
            "full_name": "Ahmed Boo",
            "email": "azizi@nextmedia.ma",
            "avatar": "https://www.gravatar.com/avatar/294a84db5511e39c441a4f51f6f3054c?s=100&d=http://api.dotshop.com/store-admin/images/generic_avatar.png",
            "phone": "11111",
            "country": "France",
            "region": "Paris",
            "city": "PAris",
            "notes": null,
            "location": "Paris, France",
            "created_at": "2021-04-08T11:17:35+00:00",
            "updated_at": "2021-04-08T11:21:08+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/d2cbe1dd-52dc-485a-8eb5-9aac08fe485e/edit"
            }
        }
    ],
    "meta": {
        "pagination": {
            "total": 8,
            "count": 8,
            "per_page": 10,
            "current_page": 1,
            "total_pages": 1,
            "links": {}
        }
    }
}
```
