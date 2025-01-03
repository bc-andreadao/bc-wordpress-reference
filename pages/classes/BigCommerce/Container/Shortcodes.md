***

# Shortcodes

Registers shortcodes for various storefront features.

This class handles:
- Shortcodes for products, cart, checkout, login, registration, account, addresses, orders, etc.
- Dependency injection for shortcode classes.
- WordPress shortcode registration.

* Full name: `\BigCommerce\Container\Shortcodes`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`PRODUCTS`|public|string|&#039;shortcode.products&#039;|
|`CART`|public|string|&#039;shortcode.cart&#039;|
|`CHECKOUT`|public|string|&#039;shortcode.checkout&#039;|
|`LOGIN`|public|string|&#039;shortcode.login&#039;|
|`REGISTER`|public|string|&#039;shortcode.register&#039;|
|`ACCOUNT`|public|string|&#039;shortcode.account&#039;|
|`ADDRESS`|public|string|&#039;shortcode.address&#039;|
|`ORDERS`|public|string|&#039;shortcode.orders&#039;|
|`GIFT_FORM`|public|string|&#039;shortcode.gift_certificate.form&#039;|
|`GIFT_BALANCE`|public|string|&#039;shortcode.gift_certificate.balance&#039;|
|`PRODUCT_REVIEWS`|public|string|&#039;shortcode.products_reviews&#039;|
|`PRODUCT_COMPONENTS`|public|string|&#039;shortcode.products_components&#039;|
|`WISHLIST`|public|string|&#039;shortcode.wishlist&#039;|


## Methods


### register

Registers all shortcodes into the DI container and attaches WordPress hooks.

```php
public register(\Pimple\Container $container): mixed
```

Services registered:
- Shortcode classes like `Products`, `Cart`, `Checkout`, etc.

Hook registered:
- `after_setup_theme`: Registers WordPress shortcodes.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The DI container for registering services. |





***


***
> Automatically generated on 2025-01-03
