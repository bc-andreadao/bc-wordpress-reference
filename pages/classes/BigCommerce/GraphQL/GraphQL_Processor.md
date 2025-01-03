***

# GraphQL_Processor

This class is responsible for handling GraphQL requests in the BigCommerce API context.

It includes methods to fetch various data types like terms, products, product reviews, and customer wishlists.
It communicates with the GraphQL API using pre-defined queries and returns the results in a structured format.
The class utilizes a configuration object for API settings and a query object for constructing GraphQL queries.

* Full name: `\BigCommerce\GraphQL\GraphQL_Processor`
* Parent class: [`\BigCommerce\GraphQL\BaseGQL`](./classes/BigCommerce/GraphQL/BaseGQL.md)



## Properties


### query



```php
protected mixed $query
```







***

## Methods


### __construct

Constructor to initialize the GraphQL processor with a configuration and query.

```php
public __construct(\BigCommerce\Api\v3\Configuration $config, mixed $query): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **\BigCommerce\Api\v3\Configuration** | The configuration object that holds API settings and other parameters. |
| `$query` | **mixed** | The GraphQL query object or string to be used for making requests. This could be an array, string, or other types depending on the implementation. |





***

### request_terms

Retrieve taxonomy terms for either categories or brands.

```php
public request_terms(string $slug, string $taxonomy = &#039;category&#039;): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$slug` | **string** | Taxonomy term slug |
| `$taxonomy` | **string** | The taxonomy type (category or brand) |





***

### request_paginated_products

Retrieve a paginated list of products.

```php
public request_paginated_products(int $size = 50): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$size` | **int** | Number of products per page (default: 50) |





***

### request_product

Retrieve a product by its slug.

```php
public request_product(string $slug): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$slug` | **string** | Product&#039;s URL slug |





***

### request_product_reviews

Retrieve product reviews for a given product.

```php
public request_product_reviews(int $product_id): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** | The product&#039;s ID |





***

### products_loop_request

Retrieve paginated product listings.

```php
public products_loop_request(int $limit = 12, string $cursor = &#039;&#039;): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$limit` | **int** | Number of products to fetch per page |
| `$cursor` | **string** | Pagination cursor (default: empty string) |





***

### get_customer_wishlist

Retrieve the wishlist for a specific customer.

```php
public get_customer_wishlist(int $customer_id, array $entityIds, bool $public = false): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customer_id` | **int** | The customer&#039;s ID |
| `$entityIds` | **array** | List of product entity IDs to fetch for wishlist |
| `$public` | **bool** | Whether to retrieve public wishlist (default: false) |





***

### get_customer_wishlists

Retrieve all wishlists for a specific customer.

```php
public get_customer_wishlists(int $customer_id): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customer_id` | **int** | The customer&#039;s ID |





***

### get_graph_ql_query_from_file

Retrieve GraphQL query from file.

```php
public get_graph_ql_query_from_file(string $file = &#039;&#039;): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$file` | **string** | The query file name (without extension) |




**Throws:**

- [`Exception`](./classes/Exception.md)



***

### get_category_tree

Retrieve the category tree.

```php
public get_category_tree(): mixed
```











**Throws:**

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***

### get_brands

Retrieve a list of brands.

```php
public get_brands(string $cursor = &#039;&#039;, int $page_size = 50): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cursor` | **string** | Pagination cursor |
| `$page_size` | **int** | Number of brands to retrieve per page |





***


## Inherited methods


### __construct

Constructor.

```php
public __construct(\BigCommerce\Api\v3\Configuration $config): mixed
```

Initializes the BaseGQL instance with the provided configuration and retrieves the tokens.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **\BigCommerce\Api\v3\Configuration** | The configuration object used for API requests. |





***

### get_channel_id

Retrieves the current channel ID from the site transient or connections.

```php
protected get_channel_id(): int
```









**Return Value:**

The channel ID.




***

### get_token

Retrieves the current GraphQL token, requesting a new one if necessary.

```php
protected get_token(): mixed
```









**Return Value:**

The current token.




***

### get_impersonation_token

Retrieves the current impersonation token, requesting a new one if necessary.

```php
protected get_impersonation_token(): mixed
```









**Return Value:**

The current impersonation token.




***

### request_im_token

Requests a new impersonation token from the API and stores it in a transient.

```php
protected request_im_token(): void
```












***

### request_token

Requests a new GraphQL token from the API and stores it in a transient.

```php
protected request_token(): void
```












***

### make_request

Makes a POST request to the GraphQL API with the provided data, headers, and URL.

```php
public make_request(mixed $data, array $headers = [], string $url = &#039;&#039;): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **mixed** | The data to send in the request body. |
| `$headers` | **array** | The headers for the request. |
| `$url` | **string** | The URL for the request. |


**Return Value:**

The parsed response data.



**Throws:**
<p>If the request fails or the response is invalid.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***

### parse_response

Parses the response from the GraphQL API.

```php
protected parse_response(array $result): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$result` | **array** | The raw response data. |


**Return Value:**

The parsed response data.



**Throws:**
<p>If the response is invalid.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***

### get_store_hash

Retrieves the store hash from the configuration host URL.

```php
protected get_store_hash(): string
```









**Return Value:**

The store hash.




***

### get_endpoint_url

Retrieves the endpoint URL for the GraphQL request.

```php
protected get_endpoint_url(): string
```









**Return Value:**

The full GraphQL endpoint URL.




***

### get_origin

Retrieves the origin (site URL) for the request.

```php
protected get_origin(): string
```









**Return Value:**

The origin URL.




***

### get_auth_bearer

Constructs the authorization bearer string for the request.

```php
protected get_auth_bearer(bool $impersonation = false): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$impersonation` | **bool** | Whether to use the impersonation token. |


**Return Value:**

The authorization header value.




***

### validate_token

Validates whether the current token is still valid and not expired.

```php
protected validate_token(): bool
```









**Return Value:**

Whether the token is valid.




***

### get_headers

Constructs the headers for the GraphQL request, including authorization.

```php
protected get_headers(bool $impersonation = false): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$impersonation` | **bool** | Whether to use the impersonation token. |


**Return Value:**

The request headers.




***


***
> Automatically generated on 2025-01-03
