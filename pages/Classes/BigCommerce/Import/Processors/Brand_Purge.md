***

# Brand_Purge

This class handles the process of purging (deleting) BigCommerce brand terms from WordPress.

It extends the base Term_Purge class and provides the specific functionality for purging brand terms.

* Full name: `\BigCommerce\Import\Processors\Brand_Purge`
* Parent class: [`\BigCommerce\Import\Processors\Term_Purge`](./classes/BigCommerce/Import/Processors/Term_Purge.md)




## Methods


### taxonomy

Get the taxonomy name for the brand purge.

```php
protected taxonomy(): string
```

This method returns the taxonomy name specific to brands in BigCommerce.







**Return Value:**

The name of the taxonomy.




***

### running_state

Get the state for the running purge process.

```php
protected running_state(): string
```

This method returns the status representing the running state of the brand purge.







**Return Value:**

The status indicating the purge process is running.




***

### completed_state

Get the state for the completed purge process.

```php
protected completed_state(): string
```

This method returns the status representing the completion of the brand purge.







**Return Value:**

The status indicating the purge process is completed.




***

### get_remote_term_ids

Get the remote term IDs for the given brand IDs.

```php
protected get_remote_term_ids(array $ids): array
```

This method fetches the brand data from the BigCommerce API using the provided brand IDs and
returns the corresponding term IDs.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$ids` | **array** | The array of BigCommerce brand IDs to retrieve. |


**Return Value:**

The array of term IDs corresponding to the provided brand IDs.




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

The taxonomy name (e.g., 'product_category', 'product_brand')




***

### running_state

Gets the status identifier for when this term purge process is running.

```php
protected running_state(): string
```




* This method is **abstract**.




**Return Value:**

The status identifier for the running state




***

### completed_state

Gets the status identifier for when this term purge process is completed.

```php
protected completed_state(): string
```




* This method is **abstract**.




**Return Value:**

The status identifier for the completed state




***

### run



```php
public run(): mixed
```












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


***
> Automatically generated on 2025-01-14
