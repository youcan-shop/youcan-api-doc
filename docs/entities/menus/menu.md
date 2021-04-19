The Menu entity at YouCan.

| Attribute Name    | Type | Description |
| -------------     | ----| --- |
| id                | string | Identifier (UUID) |
| name              | string | Name |
| slug              | string | URL slug |
| is_default        | boolean | If it is the default menu |
| links             |  array of objects [[Link](#link)], null | Array of links will display for the menu |
| links.children    |  array of objects [[Link childern](#Links children)], null | Array of links will display as sub link |

## Link

| Param Name    | Param Type    | Description                                                       |    
| ------------  | ------------- | ----------------------------------------------------------------- | 
| `id`          | uuid          | Identifier (UUID)                                                 | 
| `name`        | string        | Name of link                                                      | 
| `link`        | string        | Link path                                                         | 
| `link_to`     | smallint      | Type of link go to 1: Page, 2: Category 3: Product, 4: External   | 
| `order`       | int           | Link position                                                     | 

### Links children

| Param Name    | Param Type    | Description                                                       | 
| ------------  | ------------- | ----------------------------------------------------------------- | 
| `id`          | uuid          | Identifier (UUID)                                                 | 
| `name`        | string        | Name of link                                                      | 
| `link`        | string        | Link path                                                         | 
| `link_to`     | smallint      | Type of link go to 1: Page, 2: Category 3: Product, 4: External   | 
| `order`       | int           | Link position                                                     |