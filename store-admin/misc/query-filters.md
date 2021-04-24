# Introduction

Query filters are the parameters used to navigate the API resources, search, paginate, filter, etc.

## Search

The `q` parameter can be used to search for something under a listing in a resource. Ex:

```
/api/products?q=amazing product
```

## Pagination

The `page` parameter can be used to navigate pages in a resource listing.

```
/api/products?page=2
```

In each resource listing, the API return pagination data that can be used to traverse pages.

```json
{
  "data": {
    // ...
  },
  "meta": {
          "pagination": {
              "total": 21,
              "count": 10,
              "per_page": 10,
              "current_page": 1,
              "total_pages": 3,
              "links": {
                  "next": "https://seller-area.youcan.shop/admin/api/products?page=2"
              }
          }
      }
}
```

## Limiting Results

If you want to limit the number of rows you want to in the response, this will make your requests quicker:

```
/api/products?limit=2
```

## Sorting

To get the best results, you can sort it using the available fields for the selected resources:

```
/api/products?sort_field=name&sort_order=asc
```

By default, you get latest created data:

```
/api/products?sort_field=created_at&sort_order=desc
```

## Filters

Filters are a powerful way to narrow search results, we update this feature frequently to include more fields.

Let's say we want the list of products with inventory less than 5

```
/api/products?filters[0][field]=inventory&filters[0][operator]=<&filters[0][value]=5
```

You can also use multiple filters in one query.

```
/api/products?filters[0][field]=inventory&filters[0][operator]=<&filters[0][value]=5&filters[0][field]=trashed&filters[1][operator]==&filters[1][value]=true
```

The above request will bring products with inventory less than 5 and include deleted products too.
