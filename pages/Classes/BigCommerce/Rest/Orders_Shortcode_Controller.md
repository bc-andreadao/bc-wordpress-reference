***

# Orders_Shortcode_Controller





* Full name: `\BigCommerce\Rest\Orders_Shortcode_Controller`
* Parent class: [`\BigCommerce\Rest\Rest_Controller`](./classes/BigCommerce/Rest/Rest_Controller.md)




## Methods


### register_routes



```php
public register_routes(): mixed
```












***

### get_rendered_item_params



```php
public get_rendered_item_params(): mixed
```












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


***
> Automatically generated on 2025-01-14
