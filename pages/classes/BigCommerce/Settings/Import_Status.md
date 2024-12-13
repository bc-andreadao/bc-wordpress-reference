***

# Import_Status

Class Import_Status

Displays the import status on the settings page after the import button

* Full name: `\BigCommerce\Settings\Import_Status`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`AJAX_ACTION_IMPORT_STATUS`|public| |&#039;bigcommerce_import_status&#039;|
|`IMPORT_TOTAL_PRODUCTS`|public| |&#039;bigcommerce_import_total_products&#039;|


## Methods


### __construct



```php
public __construct(\BigCommerce\Import\Task_Manager $manager): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$manager` | **\BigCommerce\Import\Task_Manager** |  |





***

### is_parallel_run_enabled



```php
public static is_parallel_run_enabled(): false|mixed|void
```



* This method is **static**.








***

### render_status



```php
public render_status(): void
```












***

### current_status_notice

Render a notice for the status of a currently running import

```php
public current_status_notice(): void
```












***

### validate_ajax_current_status_request

Validates the nonce for the ajax request before any
more processing begins

```php
public validate_ajax_current_status_request(): void
```












***

### ajax_current_status

Returns current status as a json response

```php
public ajax_current_status(): void
```












***

### cache_queue_size

Cache the current size of the import queue.

```php
public cache_queue_size(): void
```

This allows us to show progress as the queue
diminishes.










***


***
> Automatically generated on 2024-12-13
