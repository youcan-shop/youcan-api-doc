# Login a customer

Endpoint: `https://my-store.youcan.shop/api/customers/login`

Method: `POST`

## Parameters

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| `email` | string | Customer email | yes |
| `password` | string | Customer password | yes |

## Response

[200] Ok
```json
{
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9...",
    "token_type": "bearer",
    "expires_in": 7776000
}
```

[422] Unprocessable Entity
```json
{
    "status": 422,
    "detail": "The given data was invalid.",
    "meta": {
        "fields": {
            "email": [
                "The selected email is invalid."
            ]
        }
    }
}
```
