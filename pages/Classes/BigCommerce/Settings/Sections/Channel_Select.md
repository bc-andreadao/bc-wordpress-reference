***

# Channel_Select





* Full name: `\BigCommerce\Settings\Sections\Channel_Select`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;channel_select&#039;|
|`CHANNEL_TERM`|public| |&#039;bigcommerce_channel_term_id&#039;|
|`NEW_CHANNEL`|public| |&#039;create&#039;|
|`NEW_NAME`|public| |&#039;bigcommerce_new_channel_name&#039;|


## Methods


### register_settings_section



```php
public register_settings_section(): mixed
```












***

### render_channel_select_field



```php
public render_channel_select_field(): mixed
```












***

### sanitize_channel_name

Sanitize the channel name before saving or using

```php
public sanitize_channel_name(string $name): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$name` | **string** | The channel name to sanitize |


**Return Value:**

The sanitized channel name




***

### render_field

Override parent render_field to ensure channel name is sanitized

```php
public render_field(mixed $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





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
> Automatically generated on 2025-01-14
