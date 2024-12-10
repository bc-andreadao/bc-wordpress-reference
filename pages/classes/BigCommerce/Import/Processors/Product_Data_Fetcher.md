***

# Product_Data_Fetcher





* Full name: `\BigCommerce\Import\Processors\Product_Data_Fetcher`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./Import_Processor.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STATE_OPTION`|public| |&#039;bigcommerce_import_product_id_fetcher_state&#039;|
|`FILTERED_LISTING_MAP`|public| |&#039;bigcommerce_filtered_listing_map&#039;|

## Properties


### limit



```php
private int $limit
```






***

### catalog



```php
private \BigCommerce\Api\v3\Api\CatalogApi $catalog
```






***

## Methods


### __construct

Product_Data_Fetcher constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CatalogApi $catalog, int $limit = 10): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$catalog` | **\BigCommerce\Api\v3\Api\CatalogApi** |  |
| `$limit` | **int** | Number of products to fetch per request, max of 10 per API limits |





***

### run



```php
public run(): mixed
```












***

### fetch_end



```php
private fetch_end(mixed $next, mixed $status, mixed $chunks): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$next` | **mixed** |  |
| `$status` | **mixed** |  |
| `$chunks` | **mixed** |  |





***

### get_filtered_listing_map



```php
private get_filtered_listing_map(): mixed
```












***

### get_next



```php
private get_next(): mixed
```












***

### set_next



```php
private set_next(mixed $next): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$next` | **mixed** |  |





***

### get_state



```php
private get_state(): mixed
```












***

### set_state



```php
private set_state(array $state): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$state` | **array** |  |





***

### clear_state



```php
private clear_state(): mixed
```












***

### state_option



```php
private state_option(): mixed
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

### clear_cache

Clear caches that may be storing the option

```php
private clear_cache(string $option): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |





***


***
> Automatically generated on 2024-12-10
