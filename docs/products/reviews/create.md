# Create a Product Review

Endpoint: `https://api.youcan.shop/products/{id}/reviews` 

Method: `POST`

## Parameters

- `id`: Product id

## Body

| Param Name           | Param Type    | Description           | Required |
| -------------------- | ------------- | --------------------- | -------- |
| `ratings`            | integer       | Product review ratings are between zero and five       | yes      |
| `email`        | string       | Product reviewer's email address      | yes      |
| `first_name`        | string       | Product reviewer's first name       | yes      |
| `last_name`        | string       | Product reviewer's last name       | no      |
| `content`        | string       | Product reviewer's last name       | no      |
| `images` | File[] | Product review images | no |

## Response

[201] Review successfully created

```json
{
    "id": "040f993d-76b9-4309-a63d-1fa260f817df",
    "ratings": 3,
    "first_name": "Mohamed",
    "last_name": "",
    "content": "",
    "images_urls": [],
    "created_at": "2021-04-21T12:14:50+00:00"
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

[404] Product not found