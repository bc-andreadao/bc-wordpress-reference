***

# Import





* Full name: `\BigCommerce\Settings\Sections\Import`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;import&#039;|
|`OPTION_FREQUENCY`|public| |&#039;bigcommerce_import_frequency&#039;|
|`OPTION_NEW_PRODUCTS`|public| |&#039;bigcommerce_import_new_products&#039;|
|`BATCH_SIZE`|public| |&#039;bigcommerce_import_batch_size&#039;|
|`ENABLE_PRODUCTS_WEBHOOKS`|public| |&#039;bigcommerce_import_enable_webhooks&#039;|
|`ENABLE_CUSTOMER_WEBHOOKS`|public| |&#039;bigcommerce_import_enable_customer_webhooks&#039;|
|`ENABLE_IMAGE_IMPORT`|public| |&#039;bigcommerce_import_enable_image_import&#039;|
|`MAX_CONCURRENT`|public| |&#039;bigcommerce_import_max_concurrent&#039;|
|`RUN_IN_PARALLEL`|public| |&#039;bigcommerce_parallel_run&#039;|
|`HEADLESS_FLAG`|public| |&#039;bigcommerce_headless_flag&#039;|
|`FREQUENCY_FIVE`|public| |&#039;five_minutes&#039;|
|`FREQUENCY_THIRTY`|public| |&#039;thirty_minutes&#039;|
|`FREQUENCY_HOURLY`|public| |&#039;hourly&#039;|
|`FREQUENCY_DAILY`|public| |&#039;daily&#039;|
|`FREQUENCY_WEEKLY`|public| |&#039;weekly&#039;|
|`FREQUENCY_MONTHLY`|public| |&#039;monthly&#039;|
|`FREQUENCY_NEVER`|public| |&#039;never&#039;|
|`DEFAULT_FREQUENCY`|public| |self::FREQUENCY_FIVE|
|`PRODUCT_TRANSIENT`|public| |&#039;bigcommerce_products_transient_interval&#039;|

## Properties


### options



```php
protected $options
```







***

### product_transient_groups



```php
protected $product_transient_groups
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
public register_settings_section(): void
```












***

### register_connect_channel_fields

We want just the automatic list setting to show up in the channel
selection screen during onboarding, to give the merchant a chance
to change it before the first import.

```php
public register_connect_channel_fields(): void
```












***

### section_description



```php
public section_description(): mixed
```












***

### frequency_select



```php
public frequency_select(): void
```












***

### render_gql_token_transient_settings

Render GQL token expiration options field

```php
public render_gql_token_transient_settings(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### render_products_transient_settings



```php
public render_products_transient_settings(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### new_products_toggle



```php
public new_products_toggle(): mixed
```












***

### render_import_tasks_processing



```php
public render_import_tasks_processing(): mixed
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
> Automatically generated on 2025-01-14
