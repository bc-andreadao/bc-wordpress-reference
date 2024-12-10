***

# Store_Settings





* Full name: `\BigCommerce\Import\Processors\Store_Settings`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./Import_Processor.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`DOMAIN`|public| |&#039;bigcommerce_domain&#039;|
|`MSF_FLAG`|public| |&#039;bigcommerce_multi_storefront&#039;|
|`PRODUCT_OUT_OF_STOCK`|public| |&#039;bigcommerce_product_out_of_stock_behavior&#039;|
|`OPTION_OUT_OF_STOCK`|public| |&#039;bigcommerce_settings_option_out&#039;|
|`LEGACY_OPTIONS`|public| |[&#039;product_out_of_stock_behavior&#039;, &#039;option_out_of_stock_behavior&#039;]|

## Properties


### store_api



```php
private \BigCommerce\Api\Store_Api $store_api
```






***

### default_customer_group



```php
private \BigCommerce\Import\Processors\Default_Customer_Group $default_customer_group
```






***

### storefront_processor



```php
private \BigCommerce\Import\Processors\Storefront_Processor $storefront_processor
```






***

### api_v3



```php
private \BigCommerce\Api\v3\Api\SettingsApi $api_v3
```






***

## Methods


### __construct



```php
public __construct(\BigCommerce\Api\Store_Api $store_api, \BigCommerce\Import\Processors\Default_Customer_Group $default_customer_group, \BigCommerce\Import\Processors\Storefront_Processor $storefront_processor, \BigCommerce\Api\v3\Api\SettingsApi $api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$store_api` | **\BigCommerce\Api\Store_Api** |  |
| `$default_customer_group` | **\BigCommerce\Import\Processors\Default_Customer_Group** |  |
| `$storefront_processor` | **\BigCommerce\Import\Processors\Storefront_Processor** |  |
| `$api` | **\BigCommerce\Api\v3\Api\SettingsApi** |  |





***

### run



```php
public run(): mixed
```












***

### get_legacy_inventory_settings



```php
private get_legacy_inventory_settings(): false|mixed|\stdClass|string
```












***

### process_legacy_inventory_settings

Save store inventory settings

```php
private process_legacy_inventory_settings(): mixed
```












***

### sanitize_currency_symbol_position



```php
private sanitize_currency_symbol_position(mixed $position): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$position` | **mixed** |  |





***

### sanitize_mass_unit



```php
private sanitize_mass_unit(mixed $unit): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$unit` | **mixed** |  |





***

### sanitize_length_unit



```php
private sanitize_length_unit(mixed $unit): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$unit` | **mixed** |  |





***

### extract_facebook_pixel_id



```php
private extract_facebook_pixel_id(mixed $settings): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$settings` | **mixed** |  |





***

### extract_google_analytics_id



```php
private extract_google_analytics_id(mixed $settings): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$settings` | **mixed** |  |





***

### extract_analytics_code



```php
private extract_analytics_code(mixed $settings, mixed $name): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$settings` | **mixed** |  |
| `$name` | **mixed** |  |





***

### get_max_integer_units

Get the max price integer part length to be used in the ordering by price

```php
private get_max_integer_units(): int
```












***

### is_msf_on

Is multi storefront is enabled

```php
public static is_msf_on(): bool
```



* This method is **static**.








***


***
> Automatically generated on 2024-12-10
