***

# Rest

Provides RESTful controllers and endpoints for BigCommerce integration.



* Full name: `\BigCommerce\Container\Rest`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAMESPACE_BASE`|public|string|&#039;rest.namespace&#039;|
|`VERSION`|public|string|&#039;rest.version&#039;|
|`CART_BASE`|public|string|&#039;rest.cart_base&#039;|
|`CART`|public|string|&#039;rest.cart&#039;|
|`PRODUCTS_BASE`|public|string|&#039;rest.products_base&#039;|
|`PRODUCTS`|public|string|&#039;rest.products&#039;|
|`STOREFRONT_BASE`|public|string|&#039;rest.storefront_base&#039;|
|`STOREFRONT`|public|string|&#039;rest.storefront&#039;|
|`TERMS_BASE`|public|string|&#039;rest.terms_base&#039;|
|`TERMS`|public|string|&#039;rest.terms&#039;|
|`SHORTCODE_BASE`|public|string|&#039;rest.shortcode_base&#039;|
|`SHORTCODE`|public|string|&#039;rest.shortcode&#039;|
|`ORDERS_SHORTCODE_BASE`|public|string|&#039;rest.orders_shortcode_base&#039;|
|`ORDERS_SHORTCODE`|public|string|&#039;rest.orders_shortcode&#039;|
|`COMPONENT_SHORTCODE_BASE`|public|string|&#039;rest.product_component_shortcode_base&#039;|
|`COMPONENT_SHORTCODE`|public|string|&#039;rest.product_component_shortcode&#039;|
|`REVIEW_LIST_BASE`|public|string|&#039;rest.review_list_base&#039;|
|`REVIEW_LIST`|public|string|&#039;rest.review_list&#039;|
|`PRICING_BASE`|public|string|&#039;rest.pricing_base&#039;|
|`PRICING`|public|string|&#039;rest.pricing&#039;|
|`SHIPPING_BASE`|public|string|&#039;rest.shipping_base&#039;|
|`SHIPPING`|public|string|&#039;rest.shipping&#039;|
|`COUPON_CODE_BASE`|public|string|&#039;rest.coupon_code_base&#039;|
|`COUPON_CODE`|public|string|&#039;rest.coupon_code&#039;|

## Properties


### version

The version of the REST API used by the container. It is referenced when setting up the
`VERSION` service in the container, ensuring that the API version can be applied to the various API endpoints
and controllers.

```php
private string $version
```






***

## Methods


### register

Registers services and controllers in the container and sets up REST API hooks.

```php
public register(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container instance. |





***


***
> Automatically generated on 2024-12-10
