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

## Properties


### manager



```php
private \BigCommerce\Import\Task_Manager $manager
```






***

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

### current_status



```php
private current_status(): array
```









**Return Value:**

The message describing the current import and the status string




***

### get_current_task

Get task by state. Return NULL if task is not found

```php
private get_current_task(mixed $state): \BigCommerce\Import\Task_Definition|null
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$state` | **mixed** |  |





***

### previous_status



```php
private previous_status(): array
```









**Return Value:**

The message describing the previous import and the status string




***

### next_status



```php
private next_status(): array
```









**Return Value:**

The message describing the next import and the status string




***

### cache_queue_size

Cache the current size of the import queue.

```php
public cache_queue_size(): void
```

This allows us to show progress as the queue
diminishes.










***

### get_remaining_in_queue



```php
private get_remaining_in_queue(): int
```









**Return Value:**

The number of records remaining in the import queue




***

### get_timezone_string



```php
private get_timezone_string(): mixed
```












***


***
> Automatically generated on 2024-12-10
