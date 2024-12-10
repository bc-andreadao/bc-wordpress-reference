***

# Nav_Menu

Provides dependencies and behaviors for navigation menus.



* Full name: `\BigCommerce\Container\Nav_Menu`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ITEMS`|public|string|&#039;navigation.items&#039;|
|`METABOX`|public|string|&#039;navigation.metabox&#039;|
|`CUSTOMIZER`|public|string|&#039;navigation.customizer&#039;|


## Methods


### register

Registers dependencies with the container.

```php
public register(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container. |





***

### menu_items

Registers dynamic menu items dependency and hooks.

```php
private menu_items(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container. |





***

### metabox

Registers navigation metabox dependency and hooks.

```php
private metabox(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container. |





***

### customizer

Registers navigation customizer dependency and hooks.

```php
private customizer(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container. |





***


***
> Automatically generated on 2024-12-10
