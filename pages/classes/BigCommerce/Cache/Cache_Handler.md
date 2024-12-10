***

# Cache_Handler

Cache_Handler class

Responsible for flushing the catalog API WP_Object_Cache to ensure that product information is up-to-date
from the BigCommerce catalog.

* Full name: `\BigCommerce\Cache\Cache_Handler`




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


***
> Automatically generated on 2024-12-10
