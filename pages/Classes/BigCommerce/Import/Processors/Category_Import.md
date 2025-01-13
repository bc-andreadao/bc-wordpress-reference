***

# Category_Import

Abstract class for processing term imports.

This class provides common functionality for importing terms into WordPress.
It interacts with BigCommerce's API and uses GraphQL data for creating or updating terms.

* Full name: `\BigCommerce\Import\Processors\Category_Import`
* Parent class: [`\BigCommerce\Import\Processors\Term_Import`](./classes/BigCommerce/Import/Processors/Term_Import.md)




## Methods


### taxonomy

Get the taxonomy name for this import.

```php
protected taxonomy(): string
```

This method returns the taxonomy name used for categorization, which is the product category.







**Return Value:**

The taxonomy name for product categories.




***

### running_state

Get the current running state for this import.

```php
protected running_state(): string
```

This method returns the state representing the update process for categories.







**Return Value:**

The running state constant for category updating.




***

### completed_state

Get the completed state for this import.

```php
protected completed_state(): string
```

This method returns the state representing the successful completion of the category import.







**Return Value:**

The completed state constant for category update.




***

### get_fallback_terms

Get fallback terms when GraphQL request fails.

```php
protected get_fallback_terms(): array|null
```

If GraphQL fails, this method fetches categories using the REST API as a fallback. It handles pagination
and logging for both successful and failed attempts.







**Return Value:**

An array of categories or null if no categories are retrieved.




***

### get_source_data

Get category data using GraphQL.

```php
public get_source_data(string $cursor = &#039;&#039;): array
```

This method retrieves category tree data via GraphQL, handling the response and
returning the result.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cursor` | **string** | The cursor for pagination, default is an empty string. |


**Return Value:**

The processed category data from GraphQL response.



**Throws:**
<p>Throws an exception if GraphQL request fails.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***

### parse_gql_term

Parse a term (category) for GraphQL.

```php
protected parse_gql_term(mixed $term = null): array
```

This method processes a single term, extracting the image URL and setting the
parent ID before recursively parsing any children of the term.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term` | **mixed** | The term (category) to parse. |


**Return Value:**

An array of GQL_Term_Model objects representing the term and its children.




***

### parse_term_children

Parse child terms (categories).

```php
protected parse_term_children(array& $result, mixed $children, int $parent_id): mixed
```

This method recursively processes child categories for a given parent term.
It sets the image URL and parent ID for each child before adding it to the result.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$result` | **array** | An array that will contain parsed terms. |
| `$children` | **mixed** | The child terms to parse. |
| `$parent_id` | **int** | The ID of the parent term. |





***

### get_category_data

Get category data by ID.

```php
public get_category_data(int $category_id): \BigCommerce\Api\v3\Model\CategoryResponse
```

This method retrieves category data by ID using the Catalog API.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$category_id` | **int** | The ID of the category to retrieve. |


**Return Value:**

The category data response.



**Throws:**
<p>Throws an exception if API request fails.</p>

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

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



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

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***


***
> Automatically generated on 2025-01-13
