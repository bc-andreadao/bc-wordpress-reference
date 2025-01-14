***

# Pricing_Controller





* Full name: `\BigCommerce\Rest\Pricing_Controller`
* Parent class: [`\BigCommerce\Rest\Rest_Controller`](./classes/BigCommerce/Rest/Rest_Controller.md)




## Methods


### __construct

Rest_Controller constructor.

```php
public __construct(mixed $namespace_base, mixed $version, mixed $rest_base, \BigCommerce\Api\v3\Api\PricingApi $pricing_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$namespace_base` | **mixed** |  |
| `$version` | **mixed** |  |
| `$rest_base` | **mixed** |  |
| `$pricing_api` | **\BigCommerce\Api\v3\Api\PricingApi** |  |





***

### js_config

Add data to the JS config to support pricing requests

```php
public js_config(array $config): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **array** |  |





***

### is_nonce_enabled

Nonce should always be on non-headless setup or if it is enabled via Customizer

```php
public is_nonce_enabled(): bool
```












***

### register_routes



```php
public register_routes(): mixed
```












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

### get_items_permissions_check

Checks if a given request has access to read pricing.

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

### get_collection_params

Get the query params for collections.

```php
public get_collection_params(): array
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

### format_currency

Formats a numeric value as a currency string.

```php
protected format_currency(float $value, string $empty_value = &#039;&#039;): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **float** | The currency value to format. |
| `$empty_value` | **string** | The value to return if $value is empty. Pass `null` to format anyway. |


**Return Value:**

The formatted currency string or the empty value.




***


***
> Automatically generated on 2025-01-14
