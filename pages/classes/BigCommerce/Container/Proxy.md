***

# Proxy

This class registers the proxy container that adds a Wordpress proxy layer on top of the BigCommerce API.

Sets up necessary services such as REST controllers, caching, and AMP cart controllers.

* Full name: `\BigCommerce\Container\Proxy`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACCESS`|public|string|&#039;proxy.access&#039;|
|`REST_CONTROLLER`|public|string|&#039;proxy.rest_controller&#039;|
|`CACHE`|public|string|&#039;proxy.cache&#039;|
|`PROXY_BASE`|public|string|&#039;proxy.base&#039;|
|`AMP_CART_CONTROLLER`|public|string|&#039;proxy.amp_cart_controller&#039;|
|`CACHE_PRIORITY`|public|int|10|


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


***
> Automatically generated on 2024-12-31
