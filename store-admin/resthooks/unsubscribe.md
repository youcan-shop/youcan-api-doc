# Unsubscribe from event

Endpoint: `https://api.youcan.shop/resthooks/unsubscribe/{id}`

Method: `POST`

## URL Parameters

- `id`: subscription id

## Responses

[200] Ok

```json
{
  "message": "unsubscribed from event succeed",
  "type": "success"
}
```

[404] Not Found

```json
{
  "status": 404,
  "detail": "Subscription not found",
  "meta": []
}
```