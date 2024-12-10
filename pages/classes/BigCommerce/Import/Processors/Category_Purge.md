***

# Category_Purge

This class handles the process of purging product categories. It extends the
Term_Purge class and uses the CategoriesTrees trait to manage category trees.

The purge process involves fetching category data, identifying remote term IDs,
and managing the state of the purge process.

* Full name: `\BigCommerce\Import\Processors\Category_Purge`
* Parent class: [`\BigCommerce\Import\Processors\Term_Purge`](./Term_Purge.md)




## Methods


### taxonomy

Get the taxonomy name for this purge.

```php
protected taxonomy(): string
```









**Return Value:**

The taxonomy name for product categories.




***

### running_state

Get the running state for this purge.

```php
protected running_state(): string
```









**Return Value:**

The running state constant for purging categories.




***

### completed_state

Get the completed state for this purge.

```php
protected completed_state(): string
```









**Return Value:**

The completed state constant for category purge.




***

### get_remote_term_ids

Get remote term IDs for the given category IDs.

```php
protected get_remote_term_ids(array $ids): array
```

This method fetches the term IDs from the remote BigCommerce API, using either
the MSF categories endpoint or the regular categories endpoint based on the
store settings. If no IDs are provided or the response is empty, an empty
array is returned.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$ids` | **array** | Array of category IDs to fetch remote term IDs for. |


**Return Value:**

List of remote term IDs.




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

### get_msf_categories

Get the categories in the MSF category tree.

```php
public get_msf_categories(\BigCommerce\Api\v3\Api\CatalogApi $api, array $params = []): \BigCommerce\Api\v3\Model\CategoryCollectionResponse|array
```

This method retrieves categories within the MSF category tree by fetching the tree ID,
then requesting a batch of categories from the BigCommerce API.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\v3\Api\CatalogApi** | The BigCommerce Catalog API instance. |
| `$params` | **array** | Additional parameters for the category query (optional). |


**Return Value:**

A collection of categories or an empty array.



**Throws:**
<p>Throws an exception if the API request fails.</p>

- [`ApiException`](../../Api/v3/ApiException.md)



***

### get_trees

Get all category trees associated with a given channel.

```php
public get_trees(\BigCommerce\Api\v3\Api\CatalogApi $api): array
```

This method fetches category trees from BigCommerce by retrieving the channel ID
associated with the primary connection and querying the BigCommerce API for
available category trees.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\v3\Api\CatalogApi** | The BigCommerce Catalog API instance. |


**Return Value:**

An array of category trees.



**Throws:**
<p>Throws an exception if the API request fails.</p>

- [`ApiException`](../../Api/v3/ApiException.md)



***


***
> Automatically generated on 2024-12-10
