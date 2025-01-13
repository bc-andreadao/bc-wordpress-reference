***

# Shipping_Controller





* Full name: `\BigCommerce\Rest\Shipping_Controller`
* Parent class: [`\BigCommerce\Rest\Rest_Controller`](./classes/BigCommerce/Rest/Rest_Controller.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`SHIPPING_METHOD_TYPE_PERITEM`|public| |&#039;peritem&#039;|
|`SHIPPING_METHOD_TYPE_FREE`|public| |&#039;freeshipping&#039;|
|`SHIPPING_METHOD_TYPE_USPS`|public| |&#039;endicia&#039;|
|`SHIPPING_METHOD_TYPE_WEIGHT_WEIGHT`|public| |&#039;weight&#039;|
|`SHIPPING_METHOD_TYPE_WEIGHT_TOTAL`|public| |&#039;total&#039;|


## Methods


### __construct

Rest_Controller constructor.

```php
public __construct(string $namespace_base, string $version, string $rest_base, \BigCommerce\Api\Shipping_Api $shipping_api, \BigCommerce\Api\v3\Api\CartApi $cart_api, \BigCommerce\Api\v3\Api\CheckoutApi $checkout_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$namespace_base` | **string** |  |
| `$version` | **string** |  |
| `$rest_base` | **string** |  |
| `$shipping_api` | **\BigCommerce\Api\Shipping_Api** |  |
| `$cart_api` | **\BigCommerce\Api\v3\Api\CartApi** |  |
| `$checkout_api` | **\BigCommerce\Api\v3\Api\CheckoutApi** |  |





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

### get_rendered_zones_schema



```php
public get_rendered_zones_schema(): mixed
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

### get_zones



```php
public get_zones(\WP_REST_Request $request): \WP_REST_Response|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Full details about the request. |


**Return Value:**

Response object on success, or WP_Error object on failure.




***

### get_endicia_methods



```php
public get_endicia_methods(mixed $request): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **mixed** |  |





***

### get_zone_methods



```php
public get_zone_methods(\WP_REST_Request $request): \WP_REST_Response|\WP_Error
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
> Automatically generated on 2025-01-13
