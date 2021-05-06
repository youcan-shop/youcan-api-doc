# Update the logged customer account

Endpoint: `https://my-store.youcan.shop/api/customers/account`

Method: `PUT`

## Parameters

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| `email` | string | Customer email | optional |
| `password` | string | Customer password | optional |
| `password_confirmation` | string | Customer password configuration | with password |
| `first_name` | string | Customer first name | optional |
| `last_name` | string | Customer last name | optional |
| `country` | string | Customer country | optional |
| `region` | string | Customer region | optional |
| `city` | string | Customer city | optional |
| `notes` | string | Notes | optional |

## Response

To authenticate you get the customer token for the [Login endpoint](/store-front/customers/login.md) 

[401] Unauthorized
```json
{
    "status": 401,
    "detail": "Unauthenticated.",
    "meta": []
}
```

[422] Unprocessable Entity

```json
{
    "status": 422,
    "detail": "The given data was invalid.",
    "meta": {
        "fields": {
            "first_name": [
                "The first name field is required."
            ],
            "last_name": [
                "The last name field is required."
            ],
            "phone": [
                "The phone already exists in this store."
            ],
            "email": [
                "The email already exists in this store."
            ]
        }
    }
}
```

[200] OK

```json
{
    "message": "Customer account updated successfully",
    "type": "success",
    "data": null
}
```


