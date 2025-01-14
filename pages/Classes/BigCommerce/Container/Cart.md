***

# Cart

Cart service provider for managing cart-related functionality.

The `Cart` class registers various cart-related services in the container, such as:
- Menu item for the cart
- Mini cart functionality
- Cache control for cart and checkout pages
- Buy Now functionality
- Add to Cart and Cart Recovery services
- Checkout service

The class also sets up necessary action and filter hooks to integrate these services
into the WordPress environment, ensuring that cart operations are handled effectively.

* Full name: `\BigCommerce\Container\Cart`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CART_INDICATOR`|public|string|&#039;cart.page_indicator&#039;|
|`CART_CREATOR`|public|string|&#039;cart.page_creator&#039;|
|`MENU_ITEM`|public|string|&#039;cart.menu_item&#039;|
|`MINI_CART`|public|string|&#039;cart.mini_cart&#039;|
|`CACHE_CONTROL`|public|string|&#039;cart.cache_control&#039;|
|`BUY_NOW`|public|string|&#039;cart.buy_now&#039;|
|`ADD_TO_CART`|public|string|&#039;cart.add_to_cart&#039;|
|`RECOVER_FROM_CART`|public|string|&#039;cart.recover_from_cart&#039;|
|`CHECKOUT`|public|string|&#039;cart.checkout&#039;|


## Methods


### register

Registers the cart-related services and hooks within the container.

```php
public register(\Pimple\Container $container): void
```

This method registers various cart-related services such as the menu item, mini cart, cache control,
buy now functionality, add-to-cart functionality, and checkout services within the container. It also sets up
action and filter hooks to manage cart behavior throughout the application.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container used to manage services. |





***


***
> Automatically generated on 2025-01-14
