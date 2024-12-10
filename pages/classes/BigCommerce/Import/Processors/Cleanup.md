***

# Cleanup

Handles the cleanup process for BigCommerce imports, including purging product and user transients,
cleaning up queued tasks, and flushing cache related to products and customer groups.



* Full name: `\BigCommerce\Import\Processors\Cleanup`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./Import_Processor.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CLEAN_USERS_TRANSIENT`|public|string|&#039;bigcommerce_users_transient_clean&#039;|
|`PURGE_PRODUCTS`|public|string|&#039;bigcommerce_purge_products_headless&#039;|
|`CLEAN_PRODUCTS_TRANSIENT`|public|string|&#039;bigcommerce_products_transient_clean&#039;|
|`CLEAN_POSTS_PER_PAGE`|public|int|25|


## Methods


### __construct

Cleanup constructor.

```php
public __construct(\BigCommerce\Cache\Cache_Handler $cache_handler, int $batch = self::CLEAN_POSTS_PER_PAGE): mixed
```

Initializes the cleanup process with a specified batch size and cache handler.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cache_handler` | **\BigCommerce\Cache\Cache_Handler** | Cache handler instance for cache management. |
| `$batch` | **int** | Number of records to clean up per batch. Defaults to `CLEAN_POSTS_PER_PAGE`. |





***

### run

Run the cleanup process.

```php
public run(bool $abort = false, bool $pre_import = false): mixed
```

This method performs cleanup operations such as cleaning queued tasks, purging products,
and cleaning up user transients. It also schedules additional cleanup tasks if necessary.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$abort` | **bool** | Whether to abort the cleanup process. |
| `$pre_import` | **bool** | Whether this cleanup is before or after the import. |





***

### clean_customer_group_transients

Clean customer group transients after synchronization.

```php
public clean_customer_group_transients(): void
```

This method removes transient cache related to customer groups after the sync to ensure fresh data is retrieved.










***

### refresh_products_transient

Refresh the product transient cache.

```php
public refresh_products_transient(int $offset, bool $partially = false): void
```

This method flushes the product transient cache, either partially or fully, depending on the `partially` flag.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$offset` | **int** | The number of posts to skip when fetching products. |
| `$partially` | **bool** | Whether to perform a partial cache refresh or a full refresh. |





***

### refresh_product_source

Refresh the product source cache or pre-cache for smoother initial load.

```php
public refresh_product_source(int $post_id): mixed
```

This method either refreshes the product source cache or performs a pre-cache operation to speed up the initial product load.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** | The post ID of the product to refresh or pre-cache. |





***


***
> Automatically generated on 2024-12-10
