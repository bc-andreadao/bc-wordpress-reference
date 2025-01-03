***

# Nav_Menu_Options





* Full name: `\BigCommerce\Settings\Sections\Nav_Menu_Options`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;nav_menu&#039;|
|`MENU_SELECT`|public| |&#039;bigcommerce_select_nav_menu&#039;|
|`MENU_NAME`|public| |&#039;bigcommerce_nav_menu_name&#039;|
|`ITEMS_SELECT`|public| |&#039;bigcommerce_select_menu_items&#039;|


## Methods


### register_settings_section



```php
public register_settings_section(): mixed
```












***

### menu_select

Render the nav menu select box

```php
public menu_select(mixed $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### items_select

Render the checkboxes for the menu item choices

```php
public items_select(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





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


***
> Automatically generated on 2025-01-03
