The Upsell entity at YouCan.

| Attribute Name | Type | Description |
| --- | --- | --- |
| id | string | Identifier (UUID) |
| name | string | Name |
| description | string, null | Description |
| product_id | uuid | Product id concerned by this upsell |
| product_offer_ids |  array | Array of product ids the upsell will display |
| actions | array of objects [[Action](#action)] | Yes, No buttons with their setting |
| footer | string, null | Text displayed in bottom for upsell |
| weight | int, _(default: 1)_ | The weight |
| active | int, _(default: 0)_ | Status of upsell 0: Inactive, 1: Active |

## Action

### Yes button _(btn_yes)_

| Param Name   | Param Type | Description                | Required |
| ------------ | ---------- | -------------------------- | -------- |
| `title` | string       | Button title | yes      |
| `size`      | string      | Button size small/large | yes      |
| `bg_color` | string       | Button background color       | yes      |
| `font_size` | string       | Font size of text       | yes      |
| `font_color` | string       | Font color of text       | yes      |

### No button _(btn_no)_

| Param Name   | Param Type | Description                | Required |
| ------------ | ---------- | -------------------------- | -------- |
| `title` | string       | Button title | yes      |
| `size`      | string      | Button size small/large | yes      |
| `bg_color` | string       | Button background color       | yes      |
| `font_size` | string       | Font size of text       | yes      |
| `font_color` | string       | Font color of text       | yes      |