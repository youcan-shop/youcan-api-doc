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

<a name="response"></a>

## Response

[200] OK

```json
{
    "message": "customer successfully updated",
    "http_code": 200,
    "code": "UPDATED",
    "type": "success",
    "data": null
}
```
