***

# Analytics

Handles the registration and configuration of analytics services and events for BigCommerce.

This class provides integration for popular analytics platforms like Facebook Pixel, Google Analytics, and Segment.
It also manages the registration of event tracking for actions such as adding to cart and viewing products.

* Full name: `\BigCommerce\Container\Analytics`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`FACEBOOK_PIXEL`|public|string|&#039;analytics.facebook&#039;|
|`GOOGLE_ANALYTICS`|public|string|&#039;analytics.google&#039;|
|`SEGMENT`|public|string|&#039;analytics.segment&#039;|
|`ADD_TO_CART`|public|string|&#039;analytics.events.add_to_cart&#039;|
|`VIEW_PRODUCT`|public|string|&#039;analytics.events.view_product&#039;|


## Methods


### register

Registers analytics services and events into the container

```php
public register(\Pimple\Container $container): void
```

This function registers all necessary analytics providers (Facebook Pixel, Google Analytics, Segment)
and event listeners for tracking various interactions such as add-to-cart and product views.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container. |





***

### providers

Register analytics providers

```php
private providers(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### events

Register analytics events

```php
private events(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***


***
> Automatically generated on 2024-12-10
