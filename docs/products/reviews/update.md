# Update a Review

Endpoint: `https://api.youcan.shop/reviews/{id}` 

Method: `PUT`

## URL Parameters

- `id`: Review id

## Body

| Param Name           | Param Type    | Description           | Required |
| -------------------- | ------------- | --------------------- | -------- |
| `ratings`            | integer       | Product review ratings are between zero and five       | yes      |
| `email`        | string       | Product reviewer's email address      | yes      |
| `first_name`        | string       | Product reviewer's first name       | yes      |
| `last_name`        | string       | Product reviewer's last name       | no      |
| `content`        | string       | Product reviewer's last name       | no      |
| `images` | File[] | Product review images | no |

## Responses

[200] Review successfully updated

```json
{
    "message": "Product review updated successfully",
    "http_code": 200,
    "code": "UPDATED",
    "type": "success",
    "data": null
}
```

[422] Unprocessable entity

```json
{
    "ratings": [
        "The ratings field is required."
    ]
}
```

[404] Review not found
