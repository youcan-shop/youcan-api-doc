The Menu entity at YouCan.

| Attribute Name    | Type | Description |
| -------------     | ----| --- |
| id                | string | Identifier (UUID) |
| name              | string | Name |
| slug              | string | URL slug |
| is_default        | boolean | If it is the default menu |
| links             |  array of objects [[Link](#link)], null | Array of product ids the upsell will display |
| links.children    |  array of objects [[Link childern](#Links children)], null | Array of product ids the upsell will display |

## Link

| Param Name    | Param Type    | Description               | 
| ------------  | ------------- | ------------------------- | 
| `id`          | uuid          | Identifier (UUID)         | 
| `name`        | string        | name of link              | 
| `link`        | string        | Link path                 | 
| `link_to`     | smallint      | Link to                  | 
| `order`       | int           | Link order               | 

### Links children

| Param Name    | Param Type    | Description               | 
| ------------  | ------------- | ------------------------- | 
| `id`          | uuid          | Identifier (UUID)         | 
| `name`        | string        | name of link              | 
| `link`        | string        | Link path                 | 
| `link_to`     | smallint      | Link to                   | 
| `order`       | int           | Link order               |