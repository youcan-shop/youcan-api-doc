# Update an address for a customer

Endpoint: `https://api.youcan.shop/customers/{id}/addresses/{addressId}`

Method: `PUT`

<a name="parameters"></a>

## Parameters

| Param Name     | Param Type | Description                   | Required |
| -------------- | ---------- | ----------------------------- | -------- |
| `first_name`   | string     | Address holder's first name   | no       |
| `last_name`    | string     | Address holder's last name    | no       |
| `company`      | string     | Address holder's company name | no       |
| `phone`        | string     | Address holder's phone number | no       |
| `first_line`   | string     | Address holder's first line   | no       |
| `second_line`  | string     | Address holder's second line  | no       |
| `state`        | string     | Address holder's state        | no       |
| `region`       | string     | Address holder's region       | no       |
| `city`         | string     | Address holder's city         | no       |
| `zip_code`     | string     | Address holder's postal code  | no       |
| `country_code` | string     | Address holder's country code | no       |
| `is_default`   | boolean    | Address holder's country code | no       |

<a name="response"></a>
## Response

[200] OK
