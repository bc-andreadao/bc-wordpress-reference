***

# Cart_Controller





* Full name: `\BigCommerce\Rest\Cart_Controller`
* Parent class: [`\BigCommerce\Rest\Rest_Controller`](./classes/BigCommerce/Rest/Rest_Controller.md)




## Methods


### __construct

Rest_Controller constructor.

```php
public __construct(mixed $namespace_base, mixed $version, mixed $rest_base, \BigCommerce\Api\v3\Api\CartApi $cart_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$namespace_base` | **mixed** |  |
| `$version` | **mixed** |  |
| `$rest_base` | **mixed** |  |
| `$cart_api` | **\BigCommerce\Api\v3\Api\CartApi** |  |





***

### js_config

Add data to the JS config to support cart ajax

```php
public js_config(array $config): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **array** |  |





***

### register_routes



```php
public register_routes(): mixed
```












***

### get_items



```php
public get_items(\WP_REST_Request $request): \WP_Error|\WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Full data about the request. |


**Return Value:**

Response object on success, or WP_Error object on failure.




***

### prepare_item_for_response

Prepares a cart for response.

```php
public prepare_item_for_response(\BigCommerce\Api\v3\Model\Cart $cart, \WP_REST_Request $request): \WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart` | **\BigCommerce\Api\v3\Model\Cart** | Cart object. |
| `$request` | **\WP_REST_Request** | Request object. |


**Return Value:**

Response object.




***

### create_cart_permissions_check



```php
public create_cart_permissions_check(mixed $request): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **mixed** |  |





***

### cart_id_access_check

Checks that the user's cart cookie matches the cart in the request

```php
public cart_id_access_check(\WP_REST_Request $request): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** |  |





***

### create_cart

Creates the cart with an item in it

```php
public create_cart(\WP_REST_Request $request): \WP_Error|\WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Full data about the request. |


**Return Value:**

Response object on success, or WP_Error object on failure.




***

### create_item

Adds an item to the cart.

```php
public create_item(\WP_REST_Request $request): \WP_Error|\WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Full data about the request. |


**Return Value:**

Response object on success, or WP_Error object on failure.




***

### create_postable_line_item



```php
protected create_postable_line_item(\WP_REST_Request $request): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** |  |





***

### delete_item

Deletes one item from the cart.

```php
public delete_item(\WP_REST_Request $request): \WP_Error|\WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Full data about the request. |


**Return Value:**

Response object on success, or WP_Error object on failure.




***

### update_item

Updates one item from the cart.

```php
public update_item(\WP_REST_Request $request): \WP_Error|\WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Full data about the request. |


**Return Value:**

Response object on success, or WP_Error object on failure.




***

### get_cart_item

Get the item, if the ID is valid.

```php
protected get_cart_item(string $cart_id, string $item_id): \BigCommerce\Api\v3\Model\BaseItem|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart_id` | **string** |  |
| `$item_id` | **string** |  |


**Return Value:**

Term object if ID is valid, WP_Error otherwise.




***

### get_cart_data



```php
protected get_cart_data(mixed $cart_id): \BigCommerce\Api\v3\Model\Cart
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart_id` | **mixed** |  |




**Throws:**

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***

### get_item_schema

Retrieves the response's schema, conforming to JSON Schema.

```php
public get_item_schema(): array
```









**Return Value:**

Item schema data.




***

### get_mini_cart

Render the current user's mini-cart, and return as a rest
response object

```php
public get_mini_cart(): \WP_REST_Response
```












***

### get_rendered_item_schema



```php
public get_rendered_item_schema(): mixed
```












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


***
> Automatically generated on 2025-01-13
