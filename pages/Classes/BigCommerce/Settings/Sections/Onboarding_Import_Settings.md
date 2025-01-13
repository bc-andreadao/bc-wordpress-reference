***

# Onboarding_Import_Settings





* Full name: `\BigCommerce\Settings\Sections\Onboarding_Import_Settings`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;import_settings&#039;|

## Properties


### options



```php
protected $options
```







***

## Methods


### __construct



```php
public __construct(): mixed
```












***

### register_settings_section



```php
public register_settings_section(): mixed
```












***


## Inherited methods


### render_field



```php
public render_field(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### render_number_field



```php
public render_number_field(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### get_disabled_attr_headless

Get disabled attribute if headless option is on

```php
public get_disabled_attr_headless(): string
```












***

### enable_images_import_toggle

Display images import radio toggle. Adds ability to switch between images import types

```php
public enable_images_import_toggle(array $args = []): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### render_headless_flag_import



```php
public render_headless_flag_import(): mixed
```












***

### enable_products_webhooks_toggle



```php
public enable_products_webhooks_toggle(): mixed
```












***

### enable_customer_webhooks_toggle



```php
public enable_customer_webhooks_toggle(): mixed
```












***


***
> Automatically generated on 2025-01-13
