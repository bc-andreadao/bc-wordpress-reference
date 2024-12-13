***

# Store_Settings





* Full name: `\BigCommerce\Import\Processors\Store_Settings`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./classes/BigCommerce/Import/Processors/Import_Processor.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`DOMAIN`|public| |&#039;bigcommerce_domain&#039;|
|`MSF_FLAG`|public| |&#039;bigcommerce_multi_storefront&#039;|
|`PRODUCT_OUT_OF_STOCK`|public| |&#039;bigcommerce_product_out_of_stock_behavior&#039;|
|`OPTION_OUT_OF_STOCK`|public| |&#039;bigcommerce_settings_option_out&#039;|
|`LEGACY_OPTIONS`|public| |[&#039;product_out_of_stock_behavior&#039;, &#039;option_out_of_stock_behavior&#039;]|


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

### is_msf_on

Is multi storefront is enabled

```php
public static is_msf_on(): bool
```



* This method is **static**.








***


***
> Automatically generated on 2024-12-13
