***

# Error_Log

Class Log



* Full name: `\BigCommerce\Logging\Error_Log`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`EMERGENCY`|public| |&#039;emergency&#039;|
|`ALERT`|public| |&#039;alert&#039;|
|`CRITICAL`|public| |&#039;critical&#039;|
|`ERROR`|public| |&#039;error&#039;|
|`WARNING`|public| |&#039;warning&#039;|
|`NOTICE`|public| |&#039;notice&#039;|
|`INFO`|public| |&#039;info&#039;|
|`DEBUG`|public| |&#039;debug&#039;|
|`MAX_SIZE`|public| |25|
|`ALLOWED_LOGS`|public| |[&#039;debug&#039;, &#039;webhooks&#039;, &#039;manager&#039;]|

## Properties


### log



```php
public \Monolog\Logger $log
```







***

### webhook_log



```php
public $webhook_log
```







***

### log_path



```php
public string $log_path
```







***

### log_folder_path



```php
public string $log_folder_path
```







***

## Methods


### __construct

Log constructor.

```php
public __construct(string $log_path, mixed $log_folder_path): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$log_path` | **string** | File system path to the log file |
| `$log_folder_path` | **mixed** |  |





***

### init_log

Set up the import errors log

```php
public init_log(mixed $path = &#039;&#039;): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$path` | **mixed** |  |





***

### get_log_data

Get data from log

```php
public get_log_data(): array
```












***

### truncate_log

Clean log file if it has size more than set in Troubleshooting_Diagnostics::LOG_FILE_SIZE

```php
public truncate_log(): mixed
```












***

### get_log_size_mb

Get log file size in MB

```php
public get_log_size_mb(mixed $path): float|int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$path` | **mixed** |  |





***

### log_product_import_error

Writes a log line into the log file

```php
public log_product_import_error(int $product_id, \BigCommerce\Api\v3\Api\CatalogApi $catalog_api, \Exception $exception): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** |  |
| `$catalog_api` | **\BigCommerce\Api\v3\Api\CatalogApi** |  |
| `$exception` | **\Exception** |  |





***

### log



```php
public log(mixed $level, mixed $message, mixed $context, mixed $path = &#039;&#039;): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$level` | **mixed** |  |
| `$message` | **mixed** |  |
| `$context` | **mixed** |  |
| `$path` | **mixed** |  |





***

### add_log_to_diagnostics



```php
public add_log_to_diagnostics(mixed $diagnostics): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$diagnostics` | **mixed** |  |





***


***
> Automatically generated on 2025-01-14
