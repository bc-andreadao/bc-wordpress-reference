***

# Shortcode_Controller

Class Products_Controller

REST controller to provide product information

Usage:

/wp-json/bigcommerce/v1/products

Query Args:
 - per_page: results per page, defaults to 10
 - page: which page of results, defaults to 1
 - search: search string to filter results
 - bigcommerce_category: Product category term IDs, accepts array or comma delimited term IDs
 - bigcommerce_brand: Product brand term IDs, accepts array or comma delimited term IDs
 - bigcommerce_flag: Product flag term IDs (e.g., featured, sale), accepts array or comma delimited term IDs
 - order: sort results by title. Valid values are 'asc' or 'desc' (case sensitive), defaults to 'asc'.

* Full name: `\BigCommerce\Rest\Shortcode_Controller`
* Parent class: [`\BigCommerce\Rest\Products_Controller`](./classes/BigCommerce/Rest/Products_Controller.md)




## Methods


### register_routes

Registers the REST routes for products.

```php
public register_routes(): void
```












***

### get_item_params

Retrieves the query params for the collections.

```php
public get_item_params(): array
```









**Return Value:**

Query parameters for the collection.




***

### get_rendered_item_params



```php
public get_rendered_item_params(): mixed
```












***

### get_item_permissions_check

Checks if a given request has access to read shortcodes.

```php
public get_item_permissions_check(\WP_REST_Request $request): true|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Full details about the request. |


**Return Value:**

True if the request has read access, WP_Error object otherwise.




***

### get_rendered_item_permissions_check

Checks if a given request has access to read the rendered shortcodes.

```php
public get_rendered_item_permissions_check(\WP_REST_Request $request): true|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Full details about the request. |


**Return Value:**

True if the request has read access, WP_Error object otherwise.




***

### get_item

Retrieves a single shortcode

```php
public get_item(\WP_REST_Request $request): \WP_REST_Response|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Full details about the request. |


**Return Value:**

Response object on success, or WP_Error object on failure.




***

### prepare_item_for_response

Prepares a single product output for response.

```php
public prepare_item_for_response(array $args, \WP_REST_Request $request): \WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | Shortcode args |
| `$request` | **\WP_REST_Request** | Request object. |


**Return Value:**

Response object.




***

### build_shortcode_string



```php
public build_shortcode_string(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### build_selection_shortcode_args

Translate a request into shortcode args for a product single/list

```php
protected build_selection_shortcode_args(\WP_REST_Request $request): string[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** |  |





***

### build_query_shortcode_args

Translate a request into shortcode args for a product query

```php
protected build_query_shortcode_args(\WP_REST_Request $request): string[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** |  |





***

### get_item_schema

Retrieves the response's schema, conforming to JSON Schema.

```php
public get_item_schema(): array
```









**Return Value:**

Item schema data.




***

### get_rendered_item_schema



```php
public get_rendered_item_schema(): mixed
```












***

### get_rendered_item

Retrieves a single shortcode

```php
public get_rendered_item(\WP_REST_Request $request): \WP_REST_Response|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Full details about the request. |


**Return Value:**

Response object on success, or WP_Error object on failure.




***


## Inherited methods


### __construct

Rest_Controller constructor.

```php
public __construct(string $namespace_base, string $version, string $rest_base): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$namespace_base` | **string** |  |
| `$version` | **string** |  |
| `$rest_base` | **string** |  |





***

### get_namespace



```php
protected get_namespace(): mixed
```












***

### get_base_url



```php
public get_base_url(): mixed
```












***

### parse_result



```php
protected parse_result(mixed $response, mixed $client, mixed $rest_response = true): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$response` | **mixed** |  |
| `$client` | **mixed** |  |
| `$rest_response` | **mixed** |  |





***

### register_routes

Registers the REST routes for products.

```php
public register_routes(): void
```












***

### get_items_permissions_check

Checks if a given request has access to read products.

```php
public get_items_permissions_check(\WP_REST_Request $request): true|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Full details about the request. |


**Return Value:**

True if the request has read access, WP_Error object otherwise.




***

### get_items_headless

Retrieves a collection of products for headless mode.

```php
protected get_items_headless(\WP_REST_Request $request): \WP_REST_Response|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | The request object. |


**Return Value:**

The response object or error.




***

### get_items

Retrieves a collection of products.

```php
public get_items(\WP_REST_Request $request): \WP_REST_Response|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Full details about the request. |


**Return Value:**

Response object on success, or WP_Error object on failure.




***

### get_collection_params

Retrieves the query parameters for the collection.

```php
public get_collection_params(): array
```

This function extends the default collection parameters to include product-specific filters such
as sorting order, BigCommerce ID, recent updates, and channel-specific filters.







**Return Value:**

The query parameters for retrieving a collection of products.




***

### prepare_item_for_response

Prepares a single product output for response.

```php
public prepare_item_for_response(\WP_Post $post, \WP_REST_Request $request): \WP_REST_Response
```

This function prepares a product (identified by a post ID) to be included in a REST API response.
It gathers necessary product data based on the schema and adds additional fields before returning
the response.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post` | **\WP_Post** | Post object representing the product. |
| `$request` | **\WP_REST_Request** | The request object containing additional parameters. |


**Return Value:**

Response object containing the product data.




***

### js_config

Add data to the JS config to support product requests.

```php
public js_config(array $config): array
```

This function merges product-related data such as the API URL and an AJAX nonce
into the existing JS configuration array, enabling the front-end to make
product-related requests.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **array** | The current JavaScript configuration. |


**Return Value:**

Modified JavaScript configuration with product-related data.




***

### get_content_object

Get the structured content object for a specific post.

```php
protected get_content_object(int $post_id): array
```

This function retrieves the raw content of a post and formats it according to
WordPress content filters. It also trims the content to a specified length.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** | The ID of the post for which to retrieve the content. |


**Return Value:**

An array containing the raw, formatted, and trimmed content of the post.




***

### get_image_urls

Get the URLs for the attachment in all requested sizes.

```php
protected get_image_urls(int $attachment_id, array $schema): array
```

This function returns the image URLs for all sizes specified in the schema for
a given attachment ID.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attachment_id` | **int** | The ID of the attachment. |
| `$schema` | **array** | The schema that defines the image sizes. |


**Return Value:**

An associative array containing image URLs for each size.




***

### missing_image

Return missing image data for a given size.

```php
protected missing_image(string $size): array
```

This function provides a default response for a missing image for a specified
size. It can be filtered using the `bigcommerce/rest/missing_image` filter.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$size` | **string** | The size of the image for which data is missing. |


**Return Value:**

The missing image data, including URL, width, and height.




***

### get_taxonomy_properties

Get the terms for a product's taxonomy.

```php
protected get_taxonomy_properties(int $post_id, string $taxonomy): array
```

This function retrieves the terms associated with a product for a specified
taxonomy and formats them into an array.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** | The ID of the post (product). |
| `$taxonomy` | **string** | The taxonomy for which terms are to be retrieved. |


**Return Value:**

An array of terms associated with the given taxonomy for the product.




***

### get_item_schema

Retrieves the response's schema, conforming to JSON Schema.

```php
public get_item_schema(): array
```

This function generates a JSON schema representing the structure of a product
object, including fields like `post_id`, `bigcommerce_id`, `date`, and custom
taxonomy terms. The schema can be used for validation and data modeling.







**Return Value:**

Item schema data, conforming to the JSON Schema specification.




***


***
> Automatically generated on 2025-01-14
