***

# Analytics





* Full name: `\BigCommerce\Settings\Sections\Analytics`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;analytics&#039;|
|`TRACK_BY_HOOK`|public| |&#039;bigcommerce/analytics/track_by&#039;|
|`SYNC_ANALYTICS`|public| |&#039;bigcommerce_sync_analytics&#039;|
|`FACEBOOK_PIXEL`|public| |&#039;bigcommerce_facebook_pixel_id&#039;|
|`GOOGLE_ANALYTICS`|public| |&#039;bigcommerce_google_analytics_id&#039;|
|`TRACK_PRODUCT_SKU`|public| |&#039;bigcommerce_track_product_sku&#039;|
|`SEGMENT`|public| |&#039;bigcommerce_segment_key&#039;|
|`FACEBOOK_PIXEL_NAME`|public| |&#039;Facebook Pixel&#039;|
|`GOOGLE_ANALYTICS_NAME`|public| |&#039;Google Analytics&#039;|


## Methods


### __construct



```php
public __construct(\BigCommerce\Api\Store_Api $api, \BigCommerce\Api\v3\Api\SettingsApi $api_v3): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\Store_Api** |  |
| `$api_v3` | **\BigCommerce\Api\v3\Api\SettingsApi** |  |





***

### register_settings_section



```php
public register_settings_section(): void
```












***

### render_checkbox



```php
public render_checkbox(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### update_pixel_option



```php
public update_pixel_option(string $old_value, string $new_value): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$old_value` | **string** |  |
| `$new_value` | **string** |  |





***

### update_google_option



```php
public update_google_option(string $old_value, string $new_value): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$old_value` | **string** |  |
| `$new_value` | **string** |  |





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
