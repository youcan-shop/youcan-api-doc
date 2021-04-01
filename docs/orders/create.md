# Create an Order

Endpoint: `https://api.youcan.shop/orders`

Method: `POST`

## Parameters

| Param Name                        | Param Type                  | Description                  | Required |
| --------------------------------- | --------------------------- | ---------------------------- | -------- |
| `customer_id`                     | uuid                        | Order's customer id          | yes      |
| `variants`                        | [Variant](#variant)[]       | List of order's variants     | yes      |
| `selected_shipping_estimation_id` | [compound id](#compound-id) | Selected shipping for order  | yes      |
| `shipping_address`                | [Address](#address)         | Order's shipping address     | no       |
| `payment_address`                 | [Address](#address)         | Order's billing address      | no       |
| `extra_fields`                    | object                      | Order's extra input fields   | no       |
| `coupon_id`                       | uuid                        | Coupon id                    | no       |
| `discount`                        | [Discount](#discount)       | Order discounted             | no       |
| `notes`                           | string                      | Seller notes about the order | no       |
| `tags`                            | string[]                    | List of order's tags         | no       |

<a name="variant"></a>

## Variant

| Param Name   | Param Type | Description                | Required |
| ------------ | ---------- | -------------------------- | -------- |
| `quantity`   | int        | order variant's quantity   | yes      |
| `price`      | float      | order variant's unit price | yes      |
| `variant.id` | uuid       | product variant's id       | yes      |

<a name="address"></a>

## Address

| Param Name     | Param Type | Description                   | Required |
| -------------- | ---------- | ----------------------------- | -------- |
| `is_new`       | boolean    | Is it a new address           | yes      |
| `id`           | uuid       | Address id if not new         | no       |
| `first_name`   | string     | Address holder's first name   | no       |
| `last_name`    | string     | Address holder's last name    | no       |
| `company`      | string     | Address holder's company name | no       |
| `phone`        | string     | Address holder's phone number | no       |
| `first_line`   | string     | Address' first line           | no       |
| `second_line`  | string     | Address' second line          | no       |
| `region`       | string     | Address' region               | no       |
| `city`         | string     | Address' city                 | no       |
| `zip_code`     | string     | Address' postal code          | no       |
| `country_code` | string     | Address' country code         | no       |

<a name="compound-id"></a>

## Compound id

compound ids are written in the format:
`(sr|sz)_{uuid}`.\
Example: `sr_8feb6668-4186-4194-987b-42691894036c` \
Where `sr` denotes `shipping rate` and `sz` denotes `shipping zone`.\
Use `sz` if the shipping is free and `sr` when choosing a specific shipping rate.

<a nam="discount"></a>

## Discount

| Param Name | Param Type | Description       | Required |
| ---------- | ---------- | ----------------- | -------- |
| `value`    | float      | discounted amount | yes      |
| `type`     | enum       | type of discount  | yes      |
| `reason`   | string     | discount reason   | no       |

### Discount types

`1`: Percentage.\
`2`: Fixed amount.

## Response

[201] Created

```json
{
  "id": "011857b2-00b6-47af-9f8a-41e5c98b9c0d",
  "ref": "046",
  "vat": 0,
  "total": 270,
  "notes": "a note",
  "status": 1,
  "tags": ["tag1". "tag2"],
  "extra_fields": null,
  "is_refunded_by_platform": false,
  "platform_fee": 0,
  "created_at": "2021-04-01T08:34:16+00:00",
  "updated_at": "2021-04-01T08:34:17+00:00",
  "links": {
    "self": "https://seller-area.youcan.shop/admin/orders/011857b2-00b6-47af-9f8a-41e5c98b9c0d",
    "edit": "https://seller-area.youcan.shop/admin/orders/011857b2-00b6-47af-9f8a-41e5c98b9c0d/edit"
  },
  "payment": {
    "status_text": "unpaid",
    "status": 2,
    "created_at": "2021-04-01 08:34",
    "updated_at": "2021-04-01 08:34",
    "payload": {
      "gateway": "cod"
    },
    "address": []
  },
  "shipping": {
    "status_text": "unfulfilled",
    "status": 2,
    "price": 80,
    "is_free": false,
    "tracking_number": null,
    "payload": {
      "id": "8feb6668-4186-4194-987b-42691894036c",
      "compound_id": "sr_8feb6668-4186-4194-987b-42691894036c",
      "instance_class_name": "ShippingRate",
      "name": "anibra",
      "display_name": "DHL",
      "price": 80,
      "is_free": false,
      "is_active": false
    },
    "created_at": "2021-04-01 08:34",
    "updated_at": "2021-04-01 08:34",
    "address": {
      "id": "fc580b31-5908-46fb-a146-a3e80a47b6a6",
      "first_name": "zak",
      "last_name": "anibra",
      "full_name": "zak anibra",
      "first_line": "ain chok, agdal, agdal, agdal, agdal, agdal",
      "second_line": "agdal",
      "company": "wsws",
      "phone": "+212666666666",
      "country_code": "MA",
      "country_name": "Morocco",
      "state": null,
      "region": "Grand Casablanca",
      "city": "rabablanca",
      "zip_code": "20000",
      "default": false,
      "created_at": 1617266056,
      "updated_at": 1617266056
    }
  },
  "discount": {
    "id": "b0f713fd-11e3-4e95-bbb3-c9043e14b51c",
    "value": 10,
    "type": 2,
    "reason": "something",
    "type_text": "fixed"
  },
  "refunds": [],
  "variants": [
    {
      "id": "f24b49c5-bf8c-428d-bcea-1a169d7aef06",
      "price": 200,
      "quantity": 1,
      "created_at": 1617266056,
      "updated_at": 1617266056,
      "extra_fields": [],
      "variant": {
        "id": "9ebde367-65b7-4039-b8c3-d5fd141e12d7",
        "variations": {
          "default": "default"
        },
        "options": ["default"],
        "values": ["default"],
        "price": 200,
        "compare_at_price": 250,
        "weight": 0,
        "sku": null,
        "barcode": null,
        "inventory": 5,
        "is_selected": false,
        "is_default": false,
        "image": {
          "name": null,
          "url": null
        },
        "created_at": "2021-02-26T15:30:02+00:00",
        "updated_at": "2021-03-12T09:55:11+00:00",
        "product": {
          "id": "77d2618a-2a99-4fb9-aa6d-cfe16c97971f",
          "name": "Second product",
          "slug": "product-2",
          "public_url": null,
          "thumbnail": "https://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr_md.png",
          "description": "<p>The second product</p>",
          "price": 200,
          "compare_at_price": 250,
          "cost_price": null,
          "visibility": true,
          "has_variants": false,
          "variants_count": 1,
          "variant_options": [],
          "inventory": 5,
          "track_inventory": false,
          "meta": {
            "title": "Second product",
            "description": "The second product",
            "images": [
              {
                "path": "stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr.png",
                "link": "https://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr.png"
              }
            ]
          },
          "advanced_options": {
            "enabled": false,
            "related_products": []
          },
          "created_at": "2021-02-26T15:30:02+00:00",
          "updated_at": "2021-03-31T15:19:35+00:00",
          "deleted_at": false,
          "images": [
            {
              "id": "12a83f64-ef4d-46e8-80ac-3f5b91395bf4",
              "name": "stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr.png",
              "type": 1,
              "url": "https://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr.png",
              "order": 1,
              "variations": {
                "original": "https://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr.png",
                "sm": "https://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr_sm.png",
                "md": "https://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr_md.png",
                "lg": "https://cdn.youcan.shop/stores/default/products/qhxL6LFncoN0cQG2vu91JrUTrLBUy4zTXxgdvwWr_lg.png"
              }
            }
          ]
        }
      }
    }
  ]
}
```
