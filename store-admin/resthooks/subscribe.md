# Subscribe to event

Endpoint: `https://api.youcan.shop/resthooks/subscribe`

Method: `POST`

## Body

| Param Name     | Param Type | Description                  | Required |
| -------------- | ---------- | -----------------------------| -------- |
| `target_url`   | string     | Target url                   | yes      |
| `event`        | string     | Event, supported events: `inventory.low` or `order.create` | yes      |

## Responses