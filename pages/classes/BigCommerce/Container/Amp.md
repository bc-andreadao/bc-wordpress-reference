***

# Amp

This class integrates AMP (Accelerated Mobile Pages) functionality into the BigCommerce platform.

It registers necessary services and handles template overrides, assets, and customization for AMP compatibility.
The class also provides hooks and filters for customizing the AMP-specific behavior of templates, assets, and menus.

The AMP class manages the AMP checkout redirect, template override initialization, and integration with
BigCommerce's storefront rendering system to ensure AMP-compatible pages.

* Full name: `\BigCommerce\Container\Amp`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`TEMPLATE_OVERRIDE`|public|string|&#039;amp.template_override&#039;|
|`TEMPLATE_DIRECTORY`|public|string|&#039;amp.template_directory&#039;|
|`FACTORY_OVERRIDE`|public|string|&#039;amp.controller_factory_override&#039;|
|`ASSETS`|public|string|&#039;amp.assets&#039;|
|`CUSTOMIZER_STYLES`|public|string|&#039;amp.customize_styles&#039;|
|`OVERRIDES`|public|string|&#039;amp.overrides&#039;|
|`CLASSIC`|public|string|&#039;amp.classic&#039;|
|`AMP_CART`|public|string|&#039;amp.amp_cart&#039;|
|`MENU_ITEM`|public|string|&#039;amp.cart_menu_item&#039;|
|`AMP_ADMIN_NOTICES`|public|string|&#039;amp.notices&#039;|


## Methods


### register

Registers AMP classes and callbacks.

```php
public register(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | Plugin container. |





***

### admin_notices

Sets up AMP admin notices class and callbacks.

```php
private admin_notices(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | Plugin container instance. |





***


***
> Automatically generated on 2024-12-10
