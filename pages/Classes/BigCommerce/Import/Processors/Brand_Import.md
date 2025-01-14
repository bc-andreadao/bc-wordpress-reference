***

# Brand_Import

This class handles the import process for BigCommerce brands. It extends the base Term_Import class
and provides the specific functionality for importing and updating brand terms in WordPress.



* Full name: `\BigCommerce\Import\Processors\Brand_Import`
* Parent class: [`\BigCommerce\Import\Processors\Term_Import`](./classes/BigCommerce/Import/Processors/Term_Import.md)



## Properties


### batch



```php
protected array $batch
```







***

## Methods


### taxonomy

Get the taxonomy name for the brand import.

```php
protected taxonomy(): string
```

This method returns the taxonomy name specific to brands in BigCommerce.







**Return Value:**

The name of the taxonomy.




***

### running_state

Get the state for the running process.

```php
protected running_state(): string
```

This method returns the status representing the running state of the brand import.







**Return Value:**

The status indicating the import is running.




***

### completed_state

Get the state for the completed process.

```php
protected completed_state(): string
```

This method returns the status representing the completion of the brand import.







**Return Value:**

The status indicating the import is completed.




***

### parse_gql_term

Parse the BigCommerce GraphQL term data and map it to a GQL_Term_Model.

```php
protected parse_gql_term(\stdClass|null $term = null): array
```

This method processes the raw GraphQL term data and transforms it into a standardized GQL_Term_Model object,
adjusting certain properties such as the description and image URL.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term` | **\stdClass&#124;null** | The GraphQL term data to parse. |


**Return Value:**

An array containing the GQL_Term_Model instance(s).




***

### get_source_data

Get the source data for the brand import from BigCommerce.

```php
public get_source_data(string $cursor = &#039;&#039;): array
```

This method fetches brand data from BigCommerce using GraphQL and handles the response.
If the response includes a cursor, it recursively retrieves the next set of data.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cursor` | **string** | The cursor to fetch the next set of data (optional). |


**Return Value:**

The list of brand terms fetched from the BigCommerce API.



**Throws:**
<p>If there is an error retrieving the data.</p>

- [`Exception`](./classes/Exception.md)



***

### get_fallback_terms

Get the fallback terms if GraphQL data retrieval fails.

```php
protected get_fallback_terms(): array
```

This method retrieves brand data using the Catalog API if GraphQL data cannot be fetched.
It handles pagination and ensures that all brand data is retrieved.







**Return Value:**

The list of fallback brand terms fetched from the Catalog API.




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

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



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


***
> Automatically generated on 2025-01-14
