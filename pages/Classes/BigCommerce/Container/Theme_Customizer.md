***

# Theme_Customizer

Registers theme customizer panels, sections, and styles in WordPress.

This class provides functionality for setting up customizer configurations,
adding styles, and integrating with WordPress actions such as `customize_register`.

* Full name: `\BigCommerce\Container\Theme_Customizer`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`PANEL_PRIMARY`|public|string|&#039;customizer.panel.primary&#039;|
|`SECTION_BUTTONS`|public|string|&#039;customizer.section.buttons&#039;|
|`SECTION_COLORS`|public|string|&#039;customizer.section.colors&#039;|
|`SECTION_PRODUCT_SINGLE`|public|string|&#039;customizer.section.product_single&#039;|
|`SECTION_PRODUCT_ARCHIVE`|public|string|&#039;customizer.section.product_archive&#039;|
|`SECTION_PRODUCT_CATEGORIES`|public|string|&#039;customizer.section.product_categories&#039;|
|`SECTION_CART`|public|string|&#039;customizer.section.cart&#039;|
|`SECTION_CHECKOUT`|public|string|&#039;customizer.section.checkout&#039;|
|`SECTION_BANNERS`|public|string|&#039;customizer.section.banners&#039;|
|`STYLES`|public|string|&#039;customizer.styles&#039;|


## Methods


### register

Registers customizer panels, sections, and styles in the Pimple container.

```php
public register(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | Dependency injection container. |





***


***
> Automatically generated on 2025-01-14
