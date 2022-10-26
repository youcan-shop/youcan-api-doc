# Create a Product

Endpoint: `https://api.youcan.shop/stores/ticket`

Method: `POST`

## Parameters

| Param Name | Param Type | Description                               | Required |
|------------|------------|-------------------------------------------|----------|
| `type`     | int        | Type                                      | no       |
| `subject`  | string     | A Title of the message                    | yes      |
| `content`  | string     | The description of the message            | yes      |
| ` file`    | File       | Image or a file that describe the message | no       |

<a name="variant_options"></a>
### Variant Options

Ex: `[{"type": 1, "subject": "Title", "content": "Description of the problem"]`

## Response

[201] Created

```json
{
    "message": "Ticket sent to support successfully",
    "type": "success"
}
```