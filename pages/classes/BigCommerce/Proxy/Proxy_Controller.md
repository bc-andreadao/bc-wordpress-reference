***

# Proxy_Controller

Proxy_Controller class



* Full name: `\BigCommerce\Proxy\Proxy_Controller`
* Parent class: [`WP_REST_Controller`](./classes/WP_REST_Controller.md)



## Properties


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
> Automatically generated on 2025-01-03
