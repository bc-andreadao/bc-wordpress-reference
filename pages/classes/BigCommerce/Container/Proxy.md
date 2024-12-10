***

# Proxy

This class registers the proxy container that adds a Wordpress proxy layer on top of the BigCommerce API.

Sets up necessary services such as REST controllers, caching, and AMP cart controllers.

* Full name: `\BigCommerce\Container\Proxy`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACCESS`|public|string|&#039;proxy.access&#039;|
|`REST_CONTROLLER`|public|string|&#039;proxy.rest_controller&#039;|
|`CACHE`|public|string|&#039;proxy.cache&#039;|
|`PROXY_BASE`|public|string|&#039;proxy.base&#039;|
|`AMP_CART_CONTROLLER`|public|string|&#039;proxy.amp_cart_controller&#039;|
|`CACHE_PRIORITY`|public|int|10|

## Properties


### proxy_base

The proxy base URL, set in the constructor.

```php
private string $proxy_base
```






***

## Methods


### register

Registers the container and initializes proxy-related services such as REST controller, cache, and AMP cart controller.

```php
public register(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | A container instance. |





***

### rest_controller

Sets up the REST controller container for proxy API requests.

```php
private rest_controller(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The Container instance. |





***

### cache

Sets up the cache container for proxy requests.

```php
private cache(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The Container instance. |





***

### amp_cart_controller

Sets up the AMP cart controller container for AMP-specific requests.

```php
private amp_cart_controller(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The Container instance. |





***


***
> Automatically generated on 2024-12-10
