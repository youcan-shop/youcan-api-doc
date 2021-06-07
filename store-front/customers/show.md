# Get logged in customer

Endpoint: `https://my-store.youcan.shop/api/customers/account`

Method: `GET`

## Response

To authenticate you get the customer token for the [Login endpoint](/store-front/customers/login) 

[401] Unauthorized
```json
{
    "status": 401,
    "detail": "Unauthenticated.",
    "meta": []
}
```

[200] OK

```json
{
    "id": "45d4bd7d-5a73-41bf-b392-8f83ecfabc9e",
    "first_name": "Customer",
    "last_name": "Name",
    "full_name": "Customer Name",
    "email": "email@example.com",
    "avatar": "https://www.gravatar.com/avatar/51da629dd1e2e92f2e191ad1eb8aae89?s=100&d=http://my-store.dotshop.com/store-admin/images/generic_avatar.png",
    "phone": "0600000000",
    "country": "MA",
    "region": "Fes",
    "city": "Meknes",
    "notes": "",
    "created_at": "2021-04-28T21:43:10+00:00",
    "updated_at": "2021-04-29T01:26:02+00:00"
}
```
