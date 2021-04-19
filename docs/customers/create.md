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

## Address

| Param Name     | Param Type | Description                   | Required |
| -------------- | ---------- | ----------------------------- | -------- |
| `first_name`   | string     | Address holder's first name   | no       |
| `last_name`    | string     | Address holder's last name    | no       |
| `company`      | string     | Address holder's company name | no       |
| `phone`        | string     | Address holder's phone number | no       |
| `first_line`   | string     | Address holder's first line   | no       |
| `second_line`  | string     | Address holder's second line  | no       |
| `region`       | string     | Address holder's region       | no       |
| `state`        | string     | Address holder's state       | no       |
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
}
```
