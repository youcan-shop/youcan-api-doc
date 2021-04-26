# Create a customer

Endpoint: `https://my-store.youcan.shop/api/customers`

Method: `POST`

## Parameters

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| `email` | string | Customer email | yes |
| `password` | string | Customer password | yes |
| `password_confirmation` | string | Customer password configuration | yes |
| `first_name` | string | Customer first name | non |
| `last_name` | string | Customer last name | non |
| `country` | string | Customer country | non |
| `region` | string | Customer region | non |
| `city` | string | Customer city | non |
| `notes` | string | Notes | non |

## Response

[201] Created

```json
{
  "id": "10303f69-eef7-43a2-b71e-b52c9ad9487b",
  "first_name": "Joe",
  "last_name": "Lam",
  "full_name": "Joe Lam",
  "email": "test@gmail.com",
  "avatar": "https://www.gravatar.com/avatar/1aedb8d9dc4751e229a335e371db8058?s=100&d=http://nordine.dotshop.com/store-admin/images/generic_avatar.png",
  "phone": null,
  "country": "",
  "region": "",
  "city": "",
  "notes": "",
  "location": ", ",
  "created_at": "2021-04-24T13:22:04+00:00",
  "updated_at": "2021-04-24T13:22:04+00:00",
  "deleted_at": null,
  "links": {
    "edit": "http://seller-area.dotshop.com/admin/customers/10303f69-eef7-43a2-b71e-b52c9ad9487b/edit"
  }
}
```
