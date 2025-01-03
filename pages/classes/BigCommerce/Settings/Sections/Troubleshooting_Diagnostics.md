***

# Troubleshooting_Diagnostics

Class Troubleshooting_Diagnostics



* Full name: `\BigCommerce\Settings\Sections\Troubleshooting_Diagnostics`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bigcommerce_diagnostics&#039;|
|`DIAGNOSTICS_ID`|public| |&#039;bigcommerce_diagnostics_id&#039;|
|`DIAGNOSTICS_NAME`|public| |&#039;bigcommerce_diagnostics_name&#039;|
|`ABORT_NAME`|public| |&#039;bigcommerce_diagnostics_import_abort&#039;|
|`FLUSH_USER`|public| |&#039;bigcommerce_diagnostics_cache_user&#039;|
|`FLUSH_PRODUCTS`|public| |&#039;bigcommerce_diagnostics_cache_products&#039;|
|`TEXTBOX_NAME`|public| |&#039;bigcommerce_diagnostics_output&#039;|
|`LOG_ERRORS`|public| |&#039;bigcommerce_diagnostics_log_import_errors&#039;|
|`LOG_FILE_SIZE`|public| |&#039;bigcommerce_diagnostics_log_file_size&#039;|
|`SYNC_SITE_URL`|public| |&#039;bigcommerce_diagnostics_sync_site_url&#039;|
|`USERS_TRANSIENT`|public| |&#039;bigcommerce_users_transient_interval&#039;|
|`AJAX_ACTION`|public| |&#039;bigcommerce_support_data&#039;|
|`AJAX_ACTION_IMPORT_ERRORS`|public| |&#039;bigcommerce_import_errors_log&#039;|

## Properties


### plugin_path

Plugin path

```php
protected string $plugin_path
```







***

### users_transient_groups



```php
protected $users_transient_groups
```







***

## Methods


### __construct



```php
public __construct(mixed $plugin_path): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$plugin_path` | **mixed** |  |





***

### register_settings_section



```php
public register_settings_section(): mixed
```












***

### render_flush_cache

Renders flush cache buttons

```php
public render_flush_cache(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### render_users_transient_settings

Renders users transient cache settings

```php
public render_users_transient_settings(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### render_import_abort

Renders import abort button

```php
public render_import_abort(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### render_sync_site_url



```php
public render_sync_site_url(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### render_field



```php
public render_field(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### render_enable_import_errors



```php
public render_enable_import_errors(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### render_log_file_size



```php
public render_log_file_size(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### get_diagnostics_data

Sets a wp_send_json answer for the ajax call that holds
information about the plugin and the hosting system

```php
public get_diagnostics_data(): mixed
```












***

### get_import_errors

Responds a formatted log content

```php
public get_import_errors(\BigCommerce\Logging\Error_Log $log): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$log` | **\BigCommerce\Logging\Error_Log** |  |





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
