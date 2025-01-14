***

# Term_Purge

Class Term_Purge

Deletes imported terms that no longer exist in BigCommerce

* Full name: `\BigCommerce\Import\Processors\Term_Purge`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./classes/BigCommerce/Import/Processors/Import_Processor.md)
* This class is an **Abstract class**


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STATE_OPTION`|public|string|&#039;bigcommerce_purge_terms_state&#039;|

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

Gets the WordPress taxonomy identifier that this purge processor handles.

```php
protected taxonomy(): string
```




* This method is **abstract**.




**Return Value:**

The taxonomy name (e.g., 'product_category', 'product_brand').




***

### running_state

Gets the status identifier for when this term purge process is running.

```php
protected running_state(): string
```




* This method is **abstract**.




**Return Value:**

The status identifier for the running state.




***

### completed_state

Gets the status identifier for when this term purge process is completed.

```php
protected completed_state(): string
```




* This method is **abstract**.




**Return Value:**

The status identifier for the completed state.




***

### run

Executes the term purge process.

```php
public run(): void
```

This method handles the deletion of WordPress terms that no longer exist in BigCommerce.
It processes terms in batches, comparing local terms with remote BigCommerce data.
The process tracks its state to support pagination and can be resumed if interrupted.









**Throws:**
<p>If there's an error communicating with the BigCommerce API.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



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

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



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
