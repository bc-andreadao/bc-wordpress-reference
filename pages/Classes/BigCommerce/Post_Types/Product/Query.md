***

# Query

Handles custom BigCommerce product queries in WordPress.

This class integrates with WordPress query modifications to support BigCommerce-specific
filters, sorting, and customization for product archives and search results.

* Full name: `\BigCommerce\Post_Types\Product\Query`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`UNFILTERED_QUERY_FLAG`|public| |&#039;_bigcommerce_unfiltered&#039;|


## Methods


### __construct

Query constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CatalogApi $catalog_api, \BigCommerce\Taxonomies\Product_Category\Query_Filter $filter): mixed
```

Initializes the query with the required Catalog API and filter instance.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$catalog_api` | **\BigCommerce\Api\v3\Api\CatalogApi** | Instance of the BigCommerce Catalog API. |
| `$filter` | **\BigCommerce\Taxonomies\Product_Category\Query_Filter** | Query filter for handling visibility and customizations. |





***

### filter_queries

Modifies WordPress queries to integrate BigCommerce-specific logic.

```php
public filter_queries(\WP_Query $query): void
```

This method applies custom sorting, filtering, and metadata adjustments to WordPress queries
based on BigCommerce product data and settings. It respects WordPress's native query vars
while introducing new ones like `bc-sort` for enhanced customization.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** | The WordPress query instance to modify. |





***

### filter_empty_query_vars

Removes empty query variables from the request vars to prevent unintended behavior.

```php
public filter_empty_query_vars(array $vars): array
```

For example, it prevents WordPress from interpreting empty s= parameters (left from product archive filters) as a search page request.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$vars` | **array** | Associative array of query variables. |


**Return Value:**

Filtered array of query variables.




***

### add_query_vars

Add custom query vars to WordPress.

```php
public add_query_vars(array $vars): array
```

This ensures custom query variables, such as 'bc-sort',
are recognized and not removed during request parsing.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$vars` | **array** | The list of query vars recognized by WordPress. |


**Return Value:**

Updated list of query vars.




***


***
> Automatically generated on 2025-01-14
