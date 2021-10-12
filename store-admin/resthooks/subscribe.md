# Subscribe to event

Endpoint: `https://api.youcan.shop/resthooks/subscribe`

Method: `POST`

## Body

| Param Name     | Param Type | Description                  | Required |
| -------------- | ---------- | -----------------------------| -------- |
| `target_url`   | string     | the URL which you want our API to POST to when this event occurs, mandatory                   | yes      |
| `event`        | string     | the event name that you want to hold about.<br />supported events: <ul><li>`inventory.low`</li><li>`order.create`</li></ul> | yes      |

## Responses

[200] Ok

```json
{
  "id": "8e6b019b-06de-496d-a96d-c9ee69c0ccf0"
}
```

[429] Too Many Requests

```json
{
  "status": 429,
  "detail": "This store has reached the max of subscriptions for this event.",
  "meta": []
}
```