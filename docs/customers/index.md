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

<a name="response"></a>

## Response

[200]

```json
{
    "data": [
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
        },
        {
            "id": "eb6f92e7-a33a-44de-bcd8-a390ae931bc1",
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
            "created_at": "2021-04-15T12:40:51+00:00",
            "updated_at": "2021-04-15T12:40:51+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/eb6f92e7-a33a-44de-bcd8-a390ae931bc1/edit"
            },
            "address": []
        },
        {
            "id": "72ab0ed5-03d4-4c5d-91f6-ce289ffea950",
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
            "created_at": "2021-04-15T12:40:36+00:00",
            "updated_at": "2021-04-15T12:40:36+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/72ab0ed5-03d4-4c5d-91f6-ce289ffea950/edit"
            },
            "address": [
                {
                    "id": "c78445dd-07e0-4a06-9c4c-34d7fbf4aba1",
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
                    "created_at": 1618490436,
                    "updated_at": 1618490436
                }
            ]
        },
        {
            "id": "aec1ae1b-f389-4741-ad64-e05465d147a4",
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
            "created_at": "2021-04-15T12:40:20+00:00",
            "updated_at": "2021-04-15T12:40:20+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/aec1ae1b-f389-4741-ad64-e05465d147a4/edit"
            },
            "address": [
                {
                    "id": "ace41e68-9e5d-4a92-afa5-79f30790845c",
                    "first_name": "mohamed",
                    "last_name": "address",
                    "full_name": "mohamed address",
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
                    "created_at": 1618490420,
                    "updated_at": 1618490420
                }
            ]
        },
        {
            "id": "109b3da0-cacf-4c00-8946-61888327f558",
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
            "created_at": "2021-04-15T12:35:49+00:00",
            "updated_at": "2021-04-15T12:35:49+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/109b3da0-cacf-4c00-8946-61888327f558/edit"
            },
            "address": []
        },
        {
            "id": "ef55b731-c8a7-4dcd-aec7-788265f90ca3",
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
            "created_at": "2021-04-15T12:35:37+00:00",
            "updated_at": "2021-04-15T12:35:37+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/ef55b731-c8a7-4dcd-aec7-788265f90ca3/edit"
            },
            "address": []
        },
        {
            "id": "b3a42abb-a337-41c2-8ce8-58ac9a5b1517",
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
            "created_at": "2021-04-15T12:35:07+00:00",
            "updated_at": "2021-04-15T12:35:07+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/b3a42abb-a337-41c2-8ce8-58ac9a5b1517/edit"
            },
            "address": [
                {
                    "id": "a2b88d66-c031-4f1d-a119-1a1c2c702970",
                    "first_name": "mohamed",
                    "last_name": "address",
                    "full_name": "mohamed address",
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
                    "created_at": 1618490107,
                    "updated_at": 1618490107
                }
            ]
        },
        {
            "id": "6776c708-10fd-4b31-975a-07af084e211e",
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
            "created_at": "2021-04-15T10:34:32+00:00",
            "updated_at": "2021-04-15T10:34:32+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/6776c708-10fd-4b31-975a-07af084e211e/edit"
            },
            "address": [
                {
                    "id": "f484a0b2-0962-40d7-b941-c335364401aa",
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
                    "created_at": 1618482872,
                    "updated_at": 1618484290
                }
            ]
        },
        {
            "id": "fc27864f-8f51-4fdd-b5d8-f2c465d47af4",
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
            "created_at": "2021-04-14T23:57:07+00:00",
            "updated_at": "2021-04-14T23:57:07+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/fc27864f-8f51-4fdd-b5d8-f2c465d47af4/edit"
            },
            "address": [
                {
                    "id": "5eac5014-1eb6-459c-8cf1-8e6979dd89ac",
                    "first_name": "mohamed",
                    "last_name": "AZIZI",
                    "full_name": "mohamed AZIZI",
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
                    "created_at": 1618485866,
                    "updated_at": 1618485866
                },
                {
                    "id": "6d553855-8b07-414a-b7e0-39bbec7bd110",
                    "first_name": "mohamed",
                    "last_name": "AZIZI",
                    "full_name": "mohamed AZIZI",
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
                    "created_at": 1618485815,
                    "updated_at": 1618485815
                },
                {
                    "id": "a76b7fcc-bc69-49ef-97a6-69ad74caaf04",
                    "first_name": "mohamed 2",
                    "last_name": "address 2",
                    "full_name": "mohamed 2 address 2",
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
                    "created_at": 1618485792,
                    "updated_at": 1618485792
                },
                {
                    "id": "e35defb0-da96-4597-ab28-b8acca921c61",
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
                    "created_at": 1618486674,
                    "updated_at": 1618486674
                },
                {
                    "id": "f55228be-1433-487c-a12e-e9f107cfcc71",
                    "first_name": "mohamed",
                    "last_name": "test3",
                    "full_name": "mohamed test3",
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
                    "created_at": 1618444627,
                    "updated_at": 1618485301
                }
            ]
        },
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
            "updated_at": "2021-04-15T00:09:28+00:00",
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
    ],
    "meta": {
        "pagination": {
            "total": 26,
            "count": 10,
            "per_page": 10,
            "current_page": 1,
            "total_pages": 3,
            "links": {
                "next": "http://api.dotshop.com/customers?page=2"
            }
        }
    }
}
```
