***

# Compatibility

Provides integration with various third-party services and themes, including WooCommerce, Matomo, and Akismet.

It handles the registration of necessary services, theme compatibility, and custom functionality for BigCommerce.

* Full name: `\BigCommerce\Container\Compatibility`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`TEMPLATES`|public|string|&#039;theme_compat.templates&#039;|
|`THEME`|public|string|&#039;theme_compat.theme&#039;|
|`WC_FACADE`|public|string|&#039;woo_compat.wc_facade&#039;|
|`MATOMO`|public|string|&#039;compatibility.matomo&#039;|
|`SPAM_CHECKER`|public|string|&#039;compatibility.spam_checker&#039;|


## Methods


### register

Registers the necessary services and actions for compatibility with external plugins and themes.

```php
public register(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The container to register services with. |





***

### matomo_integration



```php
private matomo_integration(mixed $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
