***

# Account_Settings





* Full name: `\BigCommerce\Settings\Sections\Account_Settings`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;accounts&#039;|
|`SUPPORT_EMAIL`|public| |&#039;bigcommerce_support_email&#039;|
|`REGISTRATION_SPAM_CHECK`|public| |&#039;bigcommerce_registration_spam_check&#039;|
|`ALLOW_GLOBAL_LOGINS`|public| |&#039;bigcommerce_allow_global_logins&#039;|


## Methods


### __construct



```php
public __construct(array $pages): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$pages` | **array** |  |





***

### register_settings_section



```php
public register_settings_section(): void
```












***

### render_registration_spam_check_field



```php
public render_registration_spam_check_field(): mixed
```












***

### render_allow_global_logins_field



```php
public render_allow_global_logins_field(): mixed
```












***

### maybe_sync_global_logins



```php
public maybe_sync_global_logins(string $old_value, string $new_value): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$old_value` | **string** |  |
| `$new_value` | **string** |  |





***

### add_default_global_logins



```php
public add_default_global_logins(): void
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

### render_page_field



```php
public render_page_field(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***


***
> Automatically generated on 2025-01-07
