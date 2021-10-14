# List subscriptions

Endpoint: `https://api.youcan.shop/resthooks/list`

Method: `GET`

## Responses

[200] Ok

```json
[
  {
    "id": "f648e8f3-746d-46a0-8b75-53252a0d7d5a",
    "event": "order.create",
    "target_url": "https://hooks.zapier.com/hooks/standard/10923067/756709b581fc4acea8e7614e8de4a8e3/"
  },
  {
    "id": "21525bb4-d3b5-481c-b6e4-b139fd87e02e",
    "event": "create_order",
    "target_url": "https://google.com"
  },
  {
    "id": "3d630ea1-2562-46ac-a611-88df3b092e89",
    "event": "create_order",
    "target_url": "https://another-test.com"
  },
  {
    "id": "67ef94a1-be92-4750-a3fa-1b46d02c8ffa",
    "event": "order.create",
    "target_url": "https://hooks.zapier.com/hooks/standard/10923067/04260ca8df6d49ea9c8258c15f6b463d/"
  },
  {
    "id": "f0ceaf61-f4f7-4e7a-927f-b82d6b34d5bb",
    "event": "new_order",
    "target_url": "https://hookb.in/1glX8dax3xCd6NOO6dLn"
  },
  {
    "id": "b9bb8564-4196-4c0a-b5a8-714df0d3c34f",
    "event": "inventory.low",
    "target_url": "https://hooks.zapier.com/hooks/standard/11057815/6055ea917052497aa9972f6313acc7c8/"
  },
  {
    "id": "61cd5df1-956b-450e-879e-de4b75ae736e",
    "event": "inventory.low",
    "target_url": "https://hookb.in/wNM1w6ynPliqJmrrJL3W"
  }
]
```