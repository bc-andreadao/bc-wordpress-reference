***

# Pages

Provides page-related services and ensures required pages exist for BigCommerce integration.



* Full name: `\BigCommerce\Container\Pages`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`REQUIRED_PAGES`|public|string|&#039;pages.required_pages&#039;|
|`CART_PAGE`|public|string|&#039;pages.cart&#039;|
|`CHECKOUT_PAGE`|public|string|&#039;pages.checkout&#039;|
|`CHECKOUT_COMPLETE_PAGE`|public|string|&#039;pages.checkout.complete&#039;|
|`LOGIN_PAGE`|public|string|&#039;pages.login&#039;|
|`REGISTRATION_PAGE`|public|string|&#039;pages.register&#039;|
|`ACCOUNT_PAGE`|public|string|&#039;pages.account&#039;|
|`ADDRESS_PAGE`|public|string|&#039;pages.address&#039;|
|`ORDERS_PAGE`|public|string|&#039;pages.orders&#039;|
|`GIFT_PURCHACE`|public|string|&#039;pages.gift_certificate.purchase&#039;|
|`GIFT_BALANCE`|public|string|&#039;pages.gift_certificate.balance&#039;|
|`SHIPPING_PAGE`|public|string|&#039;pages.shipping_returns&#039;|
|`WISHLIST_USER`|public|string|&#039;pages.wishlist.user&#039;|
|`WISHLIST_PUBLIC`|public|string|&#039;pages.wishlist.public&#039;|


## Methods


### register

Registers page-related services into the Pimple container.

```php
public register(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container. |





***


***
> Automatically generated on 2025-01-14
