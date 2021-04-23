# Errors
Every error includes a code, the HTTP status code, a short detail, and an additional meta can be used 
to help the YouCan support team investigate in your error quickly.

## Errors Types

| HTTP status | Description                                     | 
| ----------- | ---------------------------------------------- |
| 404         | The resource requested not found or deleted |
| 405         | _Method not allowed_ this error happened when the endpoint requested doesn't support the current request types |
| 422         | _Unprocessable entity_ this error happened when the request doesn't respect the validation ex: missing required field, invalid fields type|
| 500         | _500 Internal Server Error_ this error is generic happened when something got wrong in the service side while processing the request  |


### Examples

#### Not found
```json
{
    "status": 404,
    "detail": "Customer not found",
    "meta": []
}
```

### Validation error 
```json
{
    "status": 422,
    "detail": "The code field is required.",
    "meta": []
}
```

### Unsupported request type error
```json
{
    "status": 404,
    "detail": "The POST method is not supported for this route. Supported methods: GET, HEAD, PUT, DELETE.",
    "meta": []
}
```

### Internal error
```json
{
    "status": 500,
    "detail": "internal error"
}
```
