# Listing Orders

Endpoint: `https://api.youcan.shop/orders`

Method: `GET`

## Sorting

- `sort field`:
  - `ref`: Order ref
  - `total`: Order total
  - `created_at`: Order creation date

## Searching

To search in orders, add GET param `q`.

`https://api.youcan.shop/orders?q=<SEARCH_VALUE>`

### Searcheable fields

Searchable fields are matched when the field value contains the expression

- `Order ref`
- `Order notes`
- `Order extra fields`
- `Customer first name`
- `Customer last name`
- `Customer phone`
- `Customer email`

## Subresources

To include a sub-resource, add GET param `include`.
`https://api.youcan.shop/orders?include=<SUBRESOURCE>`

### Available subresources

- `customer`
- `variants`
- `payment`
- `shipping`
- `discount`
- `coupon`
- `comments`
- `refunds`
- `referenced_order`

## Response

[200]

```json
{
  "data": [
    {
      "id": "72aa7882-3898-49a8-87a2-506af3dd7320",
      "ref": "021",
      "vat": 0,
      "total": 40,
      "notes": null,
      "status": 1,
      "tags": [],
      "extra_fields": null,
      "is_refunded_by_platform": false,
      "platform_fee": 0,
      "created_at": "2021-03-17T09:42:07+00:00",
      "updated_at": "2021-03-17T10:40:42+00:00",
      "links": {
        "self": "http://seller-area.youcan.shop/admin/orders/72aa7882-3898-49a8-87a2-506af3dd7320",
        "edit": "http://seller-area.youcan.shop/admin/orders/72aa7882-3898-49a8-87a2-506af3dd7320/edit"
      },
      "payment": {
        "status_text": "pending",
        "status": 5,
        "created_at": "2021-03-17 09:42",
        "updated_at": "2021-03-17 09:42",
        "payload": {
          "gateway": "cod",
          "gateway_id": "ca700a5b-2113-4966-9e5c-bcecd5e5484e",
          "thank-you-message": "Thanks for your order",
          "note": ""
        },
        "address": []
      },
      "shipping": {
        "status_text": "UNKNOWN",
        "status": 0,
        "price": 0,
        "is_free": true,
        "tracking_number": "",
        "payload": {
          "id": "658378fb-087a-4c94-8ec6-4738a641c7e7",
          "compound_id": "sz_658378fb-087a-4c94-8ec6-4738a641c7e7",
          "instance_class_name": "YouCan\\Common\\Entities\\ShippingZone",
          "name": "Free Shipping",
          "display_name": "Free Shipping",
          "price": 0,
          "is_free": true,
          "is_active": true
        },
        "created_at": "2021-03-17 09:42",
        "updated_at": "2021-03-17 10:40",
        "address": []
      },
      "refunds": [],
      "variants": [
        {
          "id": "44c0317d-2771-48cc-9b4b-1f04fbd80033",
          "price": 40,
          "quantity": 1,
          "created_at": 1615974127,
          "updated_at": 1615977641,
          "extra_fields": [],
          "variant": {
            "id": "8a3a5a98-05a5-49c0-bff2-ef4f00d495e8",
            "variations": {
              "default": "default"
            },
            "options": ["default"],
            "values": ["default"],
            "price": 40,
            "compare_at_price": 60,
            "weight": 0,
            "sku": "",
            "barcode": "",
            "inventory": 5,
            "is_selected": false,
            "is_default": false,
            "image": {
              "name": null,
              "url": null
            },
            "created_at": "2021-02-26T15:30:02+00:00",
            "updated_at": "2021-02-26T15:30:02+00:00",
            "product": {
              "id": "d974bd63-6bad-41bf-9e5a-2bb53502d6db",
              "name": "Third product",
              "slug": "product-3",
              "public_url": null,
              "thumbnail": "http://cdn.youcan.shop/stores/default/products/MVyZpEEENXKTjbDIEbCBinIiwl2iXmtP4vpHtNHd_md.png",
              "description": "<p>The third product</p>",
              "price": 40,
              "compare_at_price": 60,
              "cost_price": null,
              "visibility": true,
              "has_variants": false,
              "variants_count": 1,
              "variant_options": [],
              "inventory": 5,
              "track_inventory": false,
              "meta": {
                "title": "Third product",
                "description": "The third product",
                "images": [
                  {
                    "path": "stores/default/products/MVyZpEEENXKTjbDIEbCBinIiwl2iXmtP4vpHtNHd.png",
                    "link": "http://cdn.youcan.shop/stores/default/products/MVyZpEEENXKTjbDIEbCBinIiwl2iXmtP4vpHtNHd.png"
                  }
                ]
              },
              "advanced_options": {
                "enabled": false,
                "related_products": []
              },
              "created_at": "2021-02-26T15:30:02+00:00",
              "updated_at": "2021-03-17T09:42:35+00:00",
              "deleted_at": false,
              "images": [
                {
                  "id": "c21dc84a-c84f-4073-b272-689b5f070cff",
                  "name": "stores/default/products/MVyZpEEENXKTjbDIEbCBinIiwl2iXmtP4vpHtNHd.png",
                  "type": 1,
                  "url": "http://cdn.youcan.shop/stores/default/products/MVyZpEEENXKTjbDIEbCBinIiwl2iXmtP4vpHtNHd.png",
                  "order": 0,
                  "variations": {
                    "original": "http://cdn.youcan.shop/stores/default/products/MVyZpEEENXKTjbDIEbCBinIiwl2iXmtP4vpHtNHd.png",
                    "sm": "http://cdn.youcan.shop/stores/default/products/MVyZpEEENXKTjbDIEbCBinIiwl2iXmtP4vpHtNHd_sm.png",
                    "md": "http://cdn.youcan.shop/stores/default/products/MVyZpEEENXKTjbDIEbCBinIiwl2iXmtP4vpHtNHd_md.png",
                    "lg": "http://cdn.youcan.shop/stores/default/products/MVyZpEEENXKTjbDIEbCBinIiwl2iXmtP4vpHtNHd_lg.png"
                  }
                }
              ]
            }
          }
        }
      ]
    }
    /* ... */
  ],
  "meta": {
    "pagination": {
      "total": 21,
      "count": 10,
      "per_page": 10,
      "current_page": 1,
      "total_pages": 3,
      "links": {
        "next": "http://seller-area.youcan.shop/admin/api/orders?page=2"
      }
    }
  }
}
```
