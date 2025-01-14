***

# Import

This class handles the import process for BigCommerce data. It includes functionality
to manage cron jobs, process various import tasks, handle batch sizes, and trigger
different import-related actions.



* Full name: `\BigCommerce\Container\Import`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CRON_MONITOR`|public|string|&#039;import.cron.monitor&#039;|
|`CRON_RUNNER`|public|string|&#039;import.cron.runner&#039;|
|`PARALLEL_RUNNER`|public|string|&#039;import.async.runner&#039;|
|`LOCK_MONITOR`|public|string|&#039;import.lock.monitor&#039;|
|`TIMEOUT`|public|string|&#039;timeout&#039;|
|`CUSTOMER_DEFAULT_GROUP`|public|string|&#039;import.customer_default_group&#039;|
|`MSF_STOREFRONT_PROCESSOR`|public|string|&#039;import.msf_storefront_processor&#039;|
|`TASK_MANAGER`|public|string|&#039;import.task_manager&#039;|
|`TASK_LIST`|public|string|&#039;import.task_list&#039;|
|`CACHE_CLEANUP`|public|string|&#039;import.cache_cleanup&#039;|
|`CHANNEL_LIST`|public|string|&#039;import.channel_list&#039;|
|`BATCH_SIZE`|public|string|&#039;import.batch_size&#039;|
|`LARGE_BATCH_SIZE`|public|string|&#039;import.large_batch_size&#039;|
|`POST_TASK_MANAGER`|public|string|&#039;import.postponed_task_manager&#039;|
|`START`|public|string|&#039;import.start&#039;|
|`LISTINGS`|public|string|&#039;import.listings&#039;|
|`CHANNEL`|public|string|&#039;import.channel&#039;|
|`PURGE_CATEGORIES`|public|string|&#039;import.purge.categories&#039;|
|`PURGE_BRANDS`|public|string|&#039;import.purge.brands&#039;|
|`CATEGORIES`|public|string|&#039;import.categories&#039;|
|`BRANDS`|public|string|&#039;import.brands&#039;|
|`RESIZE`|public|string|&#039;import.resize&#039;|
|`PRODUCTS`|public|string|&#039;import.products&#039;|
|`MARK`|public|string|&#039;import.mark_deleted&#039;|
|`QUEUE`|public|string|&#039;import.queue&#039;|
|`STORE`|public|string|&#039;import.store&#039;|
|`CURRENCIES`|public|string|&#039;import.currencies&#039;|
|`CLEANUP`|public|string|&#039;import.cleanup&#039;|
|`PRODUCT_CLEANUP`|public|string|&#039;import.product_cleanup&#039;|
|`IMPORT_STATUS`|public|string|&#039;import.import_status&#039;|
|`ERROR`|public|string|&#039;import.error&#039;|
|`IMPORT_TYPE`|public|string|&#039;import.type&#039;|
|`HEADLESS_PROCESSOR`|public|string|&#039;headless.processor&#039;|


## Methods


### register

Registers the import-related services and actions within the container.

```php
public register(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The container instance for dependency injection. |





***


***
> Automatically generated on 2025-01-14
