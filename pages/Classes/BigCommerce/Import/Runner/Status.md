***

# Status





* Full name: `\BigCommerce\Import\Runner\Status`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NOT_STARTED`|public| |&#039;not_started&#039;|
|`STARTED`|public| |&#039;started&#039;|
|`ABORTED`|public| |&#039;aborted&#039;|
|`FETCHING_LISTINGS`|public| |&#039;fetching_listings&#039;|
|`FETCHED_LISTINGS`|public| |&#039;fetched_listings&#039;|
|`INITIALIZING_CHANNEL`|public| |&#039;initializing_channel&#039;|
|`INITIALIZED_CHANNEL`|public| |&#039;initialized_channel&#039;|
|`FETCHING_PRODUCTS`|public| |&#039;fetching_products&#039;|
|`FETCHED_PRODUCTS`|public| |&#039;fetched_products&#039;|
|`MARKING_DELETED_PRODUCTS`|public| |&#039;marking_deleted_products&#039;|
|`MARKED_DELETED_PRODUCTS`|public| |&#039;marked_deleted_products&#039;|
|`PROCESSING_QUEUE`|public| |&#039;processing_queue&#039;|
|`PROCESSED_QUEUE`|public| |&#039;processed_queue&#039;|
|`CLEANING_PRODUCTS`|public| |&#039;cleaning_products&#039;|
|`CLEANED_PRODUCTS`|public| |&#039;cleaned_products&#039;|
|`FETCHING_STORE`|public| |&#039;fetching_store&#039;|
|`FETCHED_STORE`|public| |&#039;fetched_store&#039;|
|`FETCHING_CURRENCIES`|public| |&#039;fetching_currencies&#039;|
|`FETCHED_CURRENCIES`|public| |&#039;fetched_currencies&#039;|
|`CLEANING`|public| |&#039;cleaning&#039;|
|`COMPLETED`|public| |&#039;completed&#039;|
|`FAILED`|public| |&#039;failed&#039;|
|`UPDATING_CATEGORIES`|public| |&#039;updating_categories&#039;|
|`UPDATED_CATEGORIES`|public| |&#039;updated_categories&#039;|
|`UPDATING_BRANDS`|public| |&#039;updating_brands&#039;|
|`UPDATED_BRANDS`|public| |&#039;updated_brands&#039;|
|`PURGING_CATEGORIES`|public| |&#039;purging_categories&#039;|
|`PURGED_CATEGORIES`|public| |&#039;purged_categories&#039;|
|`PURGING_BRANDS`|public| |&#039;purging_brands&#039;|
|`PURGED_BRANDS`|public| |&#039;purged_brands&#039;|
|`RESIZING_IMAGES`|public| |&#039;resizing_images&#039;|
|`RESIZED_IMAGES`|public| |&#039;resized_images&#039;|
|`CURRENT_LOG`|public| |&#039;bigcommerce_current_import_status_log&#039;|
|`PREVIOUS_LOG`|public| |&#039;bigcommerce_previous_import_status_log&#039;|


## Methods


### current_status



```php
public current_status(): array
```









**Return Value:**

The `timestamp` and `status` of the last update to the current import




***

### previous_status



```php
public previous_status(): array
```









**Return Value:**

The `timestamp` and `status` of the last update to the previous import




***

### set_status

Add a status to the log for the current import. The status will be
appended to the log, even if it is the same as the current status.

```php
public set_status(string $status): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$status` | **string** |  |





***

### rotate_logs

Overwrite the previous log with the current log and empty the current log

```php
public rotate_logs(): void
```












***


## Inherited methods


### get_option



```php
protected get_option(string $option, bool $default = false): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |
| `$default` | **bool** |  |





***

### update_option



```php
protected update_option(string $option, mixed $value, bool $autoload = false): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |
| `$value` | **mixed** |  |
| `$autoload` | **bool** |  |





***

### add_option



```php
protected add_option(string $option, mixed $value, bool $autoload = false): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |
| `$value` | **mixed** |  |
| `$autoload` | **bool** |  |





***

### delete_option



```php
protected delete_option(string $option): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |





***


***
> Automatically generated on 2025-01-14
