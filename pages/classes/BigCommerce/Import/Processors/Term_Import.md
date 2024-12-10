***

# Term_Import

Abstract class for processing term imports.

This class provides common functionality for importing terms into WordPress.
It interacts with BigCommerce's API and uses GraphQL data for creating or updating terms.

* Full name: `\BigCommerce\Import\Processors\Term_Import`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./Import_Processor.md)
* This class is an **Abstract class**


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STATE_OPTION`|public|string|&#039;bigcommerce_import_terms_state&#039;|
|`BRANDS_CHECKPOINT`|public|string|&#039;bigcommerce_import_brands_checkpoint&#039;|

## Properties


### catalog_api



```php
public \BigCommerce\Api\v3\Api\CatalogApi $catalog_api
```






***

### gql_processor



```php
public \BigCommerce\GraphQL\GraphQL_Processor $gql_processor
```






***

### batch_size



```php
public int $batch_size
```






***

## Methods


### __construct

Constructor for the Term_Import class.

```php
public __construct(\BigCommerce\Api\v3\Api\CatalogApi $catalog_api, \BigCommerce\GraphQL\GraphQL_Processor $gql_processor, int $batch_size): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$catalog_api` | **\BigCommerce\Api\v3\Api\CatalogApi** | Instance of the Catalog API client. |
| `$gql_processor` | **\BigCommerce\GraphQL\GraphQL_Processor** | Instance of the GraphQL processor. |
| `$batch_size` | **int** | Number of terms to process in a single batch. |





***

### taxonomy

Get the name of the taxonomy being updated.

```php
protected taxonomy(): string
```




* This method is **abstract**.




**Return Value:**

The taxonomy name.




***

### get_fallback_terms

Get fallback terms in case the main source data is unavailable.

```php
protected get_fallback_terms(): array
```




* This method is **abstract**.




**Return Value:**

An array of fallback terms.




***

### running_state

Get the state name to set while the import is running.

```php
protected running_state(): string
```




* This method is **abstract**.




**Return Value:**

The running state name.




***

### completed_state

Get the state name to set when the import is complete.

```php
protected completed_state(): string
```




* This method is **abstract**.




**Return Value:**

The completed state name.




***

### run

Execute the term import process.

```php
public run(): void
```

This method fetches terms from the source, processes them, and updates
the import status as it progresses.










***

### do_term_import

Process and import a single term.

```php
protected do_term_import(\StdClass $term, bool $fallback = false): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term` | **\StdClass** | The term object to import. |
| `$fallback` | **bool** | Whether to use fallback data for this import. |





***

### get_source_data

Fetch term data from the source.

```php
public get_source_data(string $cursor = &#039;&#039;): array
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cursor` | **string** | Optional. A cursor for paginated results. |


**Return Value:**

The API response object.



**Throws:**
<p>If the API request fails.</p>

- [`ApiException`](../../Api/v3/ApiException.md)



***

### parse_gql_term

Parse a GraphQL term object into an array format.

```php
protected parse_gql_term(\StdClass|null $term = null): array
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term` | **\StdClass&#124;null** | The GraphQL term object. |


**Return Value:**

The parsed term data.




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

### handle_graph_ql_response

Parse a GraphQL response and handle pagination if necessary.

```php
protected handle_graph_ql_response(string $raw_response = &#039;&#039;): array|mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$raw_response` | **string** | The raw GraphQL response. |


**Return Value:**

Parsed term data or a cursor for the next page of results.




***

### get_page

Get the current page for the import process.

```php
protected get_page(): int
```









**Return Value:**

The current page number.




***

### set_page

Set the current page for the import process.

```php
protected set_page(int $page): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$page` | **int** | The page number to set. |





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
