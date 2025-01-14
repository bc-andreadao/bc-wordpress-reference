***

# Assets

Provides asset management for the BigCommerce plugin, including scripts, styles,
configuration, and localization for both the admin and frontend.



* Full name: `\BigCommerce\Container\Assets`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`PATH`|public|string|&#039;assets.path&#039;|
|`VERSION`|public|string|&#039;assets.version&#039;|
|`ADMIN_SCRIPTS`|public|string|&#039;assets.admin.scripts&#039;|
|`ADMIN_STYLES`|public|string|&#039;assets.admin.styles&#039;|
|`ADMIN_CONFIG`|public|string|&#039;assets.admin.config&#039;|
|`ADMIN_LOCALIZATIONN`|public|string|&#039;assets.admin.l10n&#039;|
|`FRONTEND_SCRIPTS`|public|string|&#039;assets.frontend.scripts&#039;|
|`FRONTEND_STYLES`|public|string|&#039;assets.frontend.styles&#039;|
|`FRONTEND_CONFIG`|public|string|&#039;assets.frontend.config&#039;|
|`FRONTEND_LOCALIZATION`|public|string|&#039;assets.frontend.l10n&#039;|
|`IMAGE_SIZES`|public|string|&#039;assets.frontend.imagesizes&#039;|


## Methods


### register

Registers assets in the dependency container.

```php
public register(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | Dependency injection container. |





***

### admin

Registers admin assets and related actions.

```php
public admin(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | Dependency injection container. |





***

### frontend

Registers frontend assets and related actions.

```php
public frontend(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | Dependency injection container. |





***


***
> Automatically generated on 2025-01-14
