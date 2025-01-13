***

# Api_Credentials





* Full name: `\BigCommerce\Settings\Sections\Api_Credentials`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;credentials&#039;|
|`OPTION_STORE_URL`|public| |&#039;bigcommerce_store_url&#039;|
|`OPTION_CLIENT_ID`|public| |&#039;bigcommerce_client_id&#039;|
|`OPTION_CLIENT_SECRET`|public| |&#039;bigcommerce_client_secret&#039;|
|`OPTION_ACCESS_TOKEN`|public| |&#039;bigcommerce_access_token&#039;|


## Methods


### register_settings_section



```php
public register_settings_section(mixed $suffix, mixed $screen): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$suffix` | **mixed** |  |
| `$screen` | **mixed** |  |





***

### render_help_text

Add a link to set up the API account

```php
public render_help_text(): void
```












***

### render_field



```php
public render_field(mixed $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### render_text

Render the field as a disabled text field without a name. Password
fields will be rendered with bullets in place of the value.

```php
protected render_text(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### filter_option_with_env



```php
public filter_option_with_env(bool|mixed $value, string $option, mixed $default): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **bool&#124;mixed** |  |
| `$option` | **string** |  |
| `$default` | **mixed** |  |





***

### do_api_settings_updated_action

Fires an action (once per pageload) when an API credential setting updates.

```php
public do_api_settings_updated_action(string $old_value, string $new_value): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$old_value` | **string** | Previous option value. |
| `$new_value` | **string** | New option value. |





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
> Automatically generated on 2025-01-13
