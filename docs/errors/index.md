# Errors
Every error includes a code, the HTTP status code, a short detail, and an additional meta can be used 
to help the YouCan support team investigate in your error quickly.

## Errors Types

| HTTP status | Description                  | 
| ----------- | -----------------------------|
| 404         | The resource requested not found       |
| 405         | Method not allowed          |
| 500         |  |


### Examples
#### Customer not found error
```json
{
    "status": 404,
    "code": 0,
    "detail": "Customer not found",
    "meta": []
}
```