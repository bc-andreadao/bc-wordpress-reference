***

# New_Account_Section





* Full name: `\BigCommerce\Settings\Sections\New_Account_Section`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bc_create_account&#039;|
|`STORE_INFO`|public| |&#039;bigcommerce_new_store_info&#039;|


## Methods


### register_settings_section



```php
public register_settings_section(): mixed
```












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

### render_state_field



```php
public render_state_field(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### render_country_field



```php
public render_country_field(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### get_countries_and_states



```php
protected get_countries_and_states(mixed $current_country): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$current_country` | **mixed** |  |





***

### validate_request



```php
public validate_request(array $submission, \WP_Error $errors): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** | The data submitted to the form |
| `$errors` | **\WP_Error** |  |





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
> Automatically generated on 2024-12-31
