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
            "id": "da4d2666-33d2-47de-881b-3dad8c4abf62",
            "first_name": "customer_first_name",
            "last_name": "customer_last_name",
            "full_name": "customer_full_name",
            "email": "customer_email",
            "avatar": "https://www.gravatar.com/avatar/f287649f7dd2d340b5e22704b3622ecd?s=100&d=http://api.dotshop.com/store-admin/images/generic_avatar.png",
            "phone": "+212706650843",
            "country": "Morocco",
            "region": "my_region",
            "city": "my_city",
            "notes": "my_",
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
                    "first_name": "customer_address_first_name",
                    "last_name": "customer_address_last_name",
                    "full_name": "customer_address_full_name",
                    "first_line": "customer_address_first_line",
                    "second_line": "customer_address_second_line",
                    "company": "customer_address_company",
                    "phone": "+212600000000",
                    "country_code": "MA",
                    "country_name": "Morocco",
                    "state": "customer_state",
                    "region": "my_region",
                    "city": "my_city",
                    "zip_code": "50000",
                    "default": true,
                    "created_at": 1618494926,
                    "updated_at": 1618494926
                }
            ]
        },
        {
            "first_name": "customer_first_name",
            "last_name": "customer_last_name",
            "full_name": "customer_full_name",
            "email": "customer_email",
            "avatar": "https://www.gravatar.com/avatar/f287649f7dd2d340b5e22704b3622ecd?s=100&d=http://api.dotshop.com/store-admin/images/generic_avatar.png",
            "phone": "+212706650843",
            "country": "Morocco",
            "region": "my_region",
            "city": "my_city",
            "notes": "my_",
            "location": "Fes, Morocco",
            "created_at": "2021-04-15T13:55:10+00:00",
            "updated_at": "2021-04-15T13:55:10+00:00",
            "deleted_at": null,
            "links": {
                "edit": "http://seller-area.dotshop.com/admin/customers/da4d2666-33d2-47de-881b-3dad8c4abf62/edit"
            },
            "address": []
        }
    ],
    "meta": {
        "pagination": {
            "total": 2,
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
