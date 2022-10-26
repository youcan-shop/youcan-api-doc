# Rest Hooks

- [Introduction](#introduction)
- [Authorization](#authorization)
- [Subscribe](#authorization)
- [Unsubscribe](#authorization)

<a name="introduction"></a>
## Introduction

#### What’s Rest Hooks  ?

REST Hooks itself is not a specification, it’s a collection of patterns that treat webhooks like subscriptions. the rest hook subscription are (created, updated or deleted) using a REST API.

With REST Hooks, the rest api is able to communicate with order apps in real time, via webhooks, without a complicated setup.

#### The REST Hooks pattern has four basic requirements :

- Mechanism to store subscriptions
- Mechanism to modify subscriptions via API
- List of event types & implementation of events
- Mechanism to send hooks

<a name="authorization"></a>
## Authorization

To able to work with Rest Hooks subscriptions, the user should have authentication token.<br />
You can follow previous [OAuth steps](/store-admin/oauth) to get an authentication token.

<a name="subscribe"></a>
## Subscribe

Subscribe is an [endpoint](/store-admin/resthooks/subscribe) allows you to set a target url for an event to send payloads of data.

#### Available events

| Event     | Description                   |
| -------------- | -----------------------------|
| `order.create`   | Subscription to all events of creating a new order. |
| `inventory.low`        | Subscription to all events who supposed to increment or decrement a product inventory.|
| `upsell.accept`        | Subscription to event when customer accepts upsell.|

<a name="unsubscribe"></a>
## Unsubscribe

Unsubscribe is an [endpoint](/store-admin/resthooks/unsubscribe) allows to stop a subscription for an event immediately.
