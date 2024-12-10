***

# Cache_Handler

Cache_Handler class

Responsible for flushing the catalog API WP_Object_Cache to ensure that product information is up-to-date
from the BigCommerce catalog.

* Full name: `\BigCommerce\Cache\Cache_Handler`



## Properties


### catalog_path

The catalog API path for products.

```php
private string $catalog_path
```






***

### header_params

The default HTTP header parameters used for API requests.

```php
private array $header_params
```






***

### product_response_type

The type of response expected from the API for product requests.

```php
private string $product_response_type
```






***

### group_key

The group key used in WordPress object caching for BigCommerce API data.

```php
private string $group_key
```






***

## Methods


### flush_product_catalog_object_cache

Flushes the WordPress object cache for the product catalog.

```php
public flush_product_catalog_object_cache(int $product_id, array $query_params = []): void
```

This method ensures that the cache is cleared for the specified product, allowing fresh product information
to be retrieved from the BigCommerce catalog.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** | The ID of the product to flush the cache for. |
| `$query_params` | **array** | Optional query parameters to customize the cache key. |





***

### build_serialized_key

Builds a serialized cache key for a product based on product ID and query parameters.

```php
private build_serialized_key(int $product_id, array $query_params = []): string
```

This method generates a unique cache key used to store and retrieve the product's data from the cache.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** | The ID of the product. |
| `$query_params` | **array** | Optional query parameters to customize the cache key. |


**Return Value:**

The generated cache key.




***


***
> Automatically generated on 2024-12-10
