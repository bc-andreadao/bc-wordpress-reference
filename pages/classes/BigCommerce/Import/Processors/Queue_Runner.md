***

# Queue_Runner





* Full name: `\BigCommerce\Import\Processors\Queue_Runner`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./Import_Processor.md)



## Properties


### catalog



```php
private \BigCommerce\Api\v3\Api\CatalogApi $catalog
```






***

### batch



```php
private int $batch
```






***

### max_attempts



```php
private int $max_attempts
```






***

## Methods


### __construct

Queue_Runner constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CatalogApi $catalog, int $batch = 5, int $max_attempts = 10): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$catalog` | **\BigCommerce\Api\v3\Api\CatalogApi** |  |
| `$batch` | **int** |  |
| `$max_attempts` | **int** |  |





***

### run



```php
public run(): mixed
```












***

### handle_record



```php
private handle_record(object $record, \WP_Term[] $channels): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$record` | **object** |  |
| `$channels` | **\WP_Term[]** |  |





***

### handle_update



```php
private handle_update(mixed $bigcommerce_id, mixed $data, mixed $channels = []): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bigcommerce_id` | **mixed** |  |
| `$data` | **mixed** |  |
| `$channels` | **mixed** |  |





***

### handle_update_for_channel



```php
private handle_update_for_channel(\BigCommerce\Api\v3\Model\Product $product, object[] $listings, \WP_Term $channel_term): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Api\v3\Model\Product** |  |
| `$listings` | **object[]** |  |
| `$channel_term` | **\WP_Term** |  |





***

### handle_delete



```php
private handle_delete(object $data, \WP_Term[] $channels = []): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **object** |  |
| `$channels` | **\WP_Term[]** |  |





***

### mark_task_complete



```php
private mark_task_complete(mixed $record_id, mixed $wpdb): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$record_id` | **mixed** |  |
| `$wpdb` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
