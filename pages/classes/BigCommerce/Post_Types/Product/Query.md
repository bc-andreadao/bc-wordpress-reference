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

## Properties


### query_filter



```php
private $query_filter
```






***

### catalog_api



```php
private \BigCommerce\Api\v3\Api\CatalogApi $catalog_api
```






***

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

### handle_non_visible_categories



```php
private handle_non_visible_categories(): string
```












***

### get_ordering_decimal_format

Get the Decimal Data Type Characteristics for Decimal price ordering

```php
private get_ordering_decimal_format(): string
```












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

### get_query_var_as_array



```php
private get_query_var_as_array(\WP_Query $query, mixed $var): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |
| `$var` | **mixed** |  |





***

### bcids_to_post_ids

Convert an array of BigCommerce IDs to post IDs

```php
private bcids_to_post_ids(int[] $bcids): int[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bcids` | **int[]** |  |





***

### skus_to_post_ids

Convert an array of BigCommerce SKUs to post IDs

```php
private skus_to_post_ids(string[] $skus): int[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$skus` | **string[]** |  |





***

### is_product_search



```php
private is_product_search(\WP_Query $query): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |





***

### is_product_query



```php
private is_product_query(\WP_Query $query): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |





***

### search_to_post_ids

Product search should match title, BigCommerce ID, or SKU

```php
private search_to_post_ids(string $search_phrase, mixed $is_headless = false): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$search_phrase` | **string** |  |
| `$is_headless` | **mixed** |  |





***

### perform_headless_search

Perform a search via Rest API. Retrieves an array of product ids from api
and tries to find existing product in WP DB

```php
private perform_headless_search(string $search_phrase = &#039;&#039;): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$search_phrase` | **string** |  |





***


***
> Automatically generated on 2024-12-10
