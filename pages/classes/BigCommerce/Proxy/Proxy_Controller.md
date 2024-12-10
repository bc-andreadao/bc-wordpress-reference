***

# Proxy_Controller

Proxy_Controller class



* Full name: `\BigCommerce\Proxy\Proxy_Controller`
* Parent class: [`WP_REST_Controller`](../../WP_REST_Controller.md)



## Properties


### config

Configuration

```php
private array $config
```






***

### proxy_base

Proxy base namespace.

```php
protected string $proxy_base
```






***

## Methods


### __construct

Proxy_Controller class constructor

```php
public __construct(array $config): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **array** | Configuration details. |





***

### register_routes

Init Proxy endpoints.

```php
public register_routes(): void
```












***

### create_cart

Creates a new cart and returns the BigCommerce API response.

```php
public create_cart(\WP_REST_Request $request): \WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | The request instance. |





***

### create_redirect_url

Creates redirect URLs from a cart ID.

```php
public create_redirect_url(\WP_REST_Request $request): \WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Request instance. |





***

### delete_cart

Deletes a cart.

```php
public delete_cart(\WP_REST_Request $request): \WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Request instance. |





***

### update_cart_item

Updates or deletes a cart line item.

```php
public update_cart_item(\WP_REST_Request $request): \WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Request instance. |





***

### add_cart_items

Add cart line items.

```php
public add_cart_items(\WP_REST_Request $request): \WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Request instance. |





***

### get_request_headers

Provides request headers for use in multiple methods.

```php
public get_request_headers(\WP_REST_Request $request, string $route): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | The request instance. |
| `$route` | **string** | The BigCommerce request route. |


**Return Value:**

A headers associative array.




***

### get_items_permissions_check

Permission check for REST requests to the proxy endpoint.

```php
public get_items_permissions_check(\WP_REST_Request $request): \WP_Error|true
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | REST request to check. |


**Return Value:**

True if the request is allowed, or else an error.




***

### get_items

Proxy requests.

```php
public get_items(\WP_REST_Request $request): \WP_REST_Response|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Proxied request. |





***

### filter_out_fields

Filters specified fields out of an array of data.

```php
private filter_out_fields(array $data, array $exclude_fields): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **array** | Data to filter. |
| `$exclude_fields` | **array** | Fields to exclude, by key. |


**Return Value:**

Filtered data.




***

### filter_excluded_product_fields

Filters fields out of product data.

```php
private filter_excluded_product_fields(array $product): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **array** | Product data. |


**Return Value:**

Filtered data.




***

### filter_excluded_variant_fields

Filters fields out of a variant.

```php
private filter_excluded_variant_fields(array $variant, array|null $product_data = null): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$variant` | **array** | Variant data. |
| `$product_data` | **array&#124;null** | Optionally passed in data for the variant&#039;s associated product. |


**Return Value:**

Filtered data.




***

### filter_excluded_image_fields

Filters fields out of image data.

```php
private filter_excluded_image_fields(array $image): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$image` | **array** | Image data. |


**Return Value:**

Filtered data.




***

### filter_excluded_review_fields

Filters fields out of review data.

```php
private filter_excluded_review_fields(array $review): array|null
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$review` | **array** | Review data. |


**Return Value:**

Filtered data or null if the idea review should be filtered out.




***

### filter_excluded_category_fields

Filters fields out of category data.

```php
private filter_excluded_category_fields(array $category): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$category` | **array** | Category data. |


**Return Value:**

Filtered data.




***

### filter_excluded_fields

Provides blacklisted fields for the given request route.

```php
private filter_excluded_fields(string $route, array $data): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$route` | **string** | WP REST request route. |
| `$data` | **array** | Data to filter. |


**Return Value:**

Exclude fields parameter or an empty array if nothing to exclude.




***

### route

Given a request, return the real URL.

```php
public route(\WP_REST_Request $request): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | The request. |





***


***
> Automatically generated on 2024-12-10
