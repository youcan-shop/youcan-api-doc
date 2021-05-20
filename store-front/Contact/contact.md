# Create a customer

Endpoint: `https://my-store.youcan.shop/api/contact`

Method: `POST`

## Parameters

| Param Name | Param Type | Description | Required |
| --- | --- | --- | --- |
| `email` | string |  Email address | yes |
| `subject` | string | Subject of the contact email | yes |
| `message` | string | Message | yes |

## Response

[200] OK

```json
{
  "status": 200,
  "detail": "your message has been sent successfully.",
  "meta": []
}
```

[500] Error 

```json
{
    "status": 500,
    "detail": "internal error occurred",
    "meta": []
}
```
