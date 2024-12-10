***

# Term_Purge

Class Term_Purge

Deletes imported terms that no longer exist in BigCommerce

* Full name: `\BigCommerce\Import\Processors\Term_Purge`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./Import_Processor.md)
* This class is an **Abstract class**


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STATE_OPTION`|public| |&#039;bigcommerce_purge_terms_state&#039;|

## Properties


### catalog_api



```php
public \BigCommerce\Api\v3\Api\CatalogApi $catalog_api
```






***

### batch_size



```php
public int $batch_size
```






***

## Methods


### __construct

Category_Import constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CatalogApi $catalog_api, int $batch_size): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$catalog_api` | **\BigCommerce\Api\v3\Api\CatalogApi** |  |
| `$batch_size` | **int** |  |





***

### taxonomy



```php
protected taxonomy(): string
```




* This method is **abstract**.




**Return Value:**

The name of the taxonomy to update




***

### running_state



```php
protected running_state(): string
```




* This method is **abstract**.




**Return Value:**

The name of the state to set while the import is running




***

### completed_state



```php
protected completed_state(): string
```




* This method is **abstract**.




**Return Value:**

The name of the state to set when the import is complete




***

### run



```php
public run(): mixed
```












***

### get_local_term_ids

Get the IDs of all previously imported terms

```php
private get_local_term_ids(int $page): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$page` | **int** |  |





***

### get_remote_term_ids

Get the IDs of all terms found in the API that match
the known terms

```php
protected get_remote_term_ids(int[] $ids): int[]
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$ids` | **int[]** | The IDs of terms to check against |




**Throws:**

- [`ApiException`](../../Api/v3/ApiException.md)



***

### get_page



```php
private get_page(): mixed
```












***

### set_page



```php
private set_page(mixed $page): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$page` | **mixed** |  |





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
