# Update a customer account

Endpoint: `https://my-store.youcan.shop/api/customers/account`

Method: `PUT`

## Parameters

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| `email` | string | Customer email | yes |
| `password` | string | Customer password | yes |
| `first_name` | string | Customer first name | yes |
| `last_name` | string | Customer last name | yes |
| `country` | string | Customer country | non |
| `region` | string | Customer region | non |
| `city` | string | Customer city | non |
| `notes` | string | Notes | non |

## Responses

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


