***

# Setup_Status

Class Setup_Status

Gets information about the current setup state of the BigCommerce store

* Full name: `\BigCommerce\Merchant\Setup_Status`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STATUS_CACHE`|public| |&#039;bigcommerce_store_setup_status&#039;|
|`STATUS_CACHE_TTL`|public| |&#039;600&#039;|

## Properties


### factory



```php
private \BigCommerce\Api_Factory $factory
```






***

## Methods


### __construct



```php
public __construct(\BigCommerce\Api_Factory $factory): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$factory` | **\BigCommerce\Api_Factory** |  |





***

### get_current_status

Get the current status of the store. Results
are cached in a transient for up to 10 minutes.

```php
public get_current_status(): array
```












***

### refresh_status

Refresh the status cache with new data

```php
public refresh_status(): array
```












***

### get_shipping_zone_count



```php
private get_shipping_zone_count(): mixed
```












***

### get_shipping_method_count



```php
private get_shipping_method_count(): mixed
```












***

### get_tax_class_count



```php
private get_tax_class_count(): mixed
```












***

### get_payment_methods_count



```php
private get_payment_methods_count(): mixed
```












***

### is_ssl

Indicates whether the WordPress site is using SSL
and sitewide https is enabled in the store.

```php
public is_ssl(): bool
```












***

### get_store_sitewidehttps_enabled



```php
private get_store_sitewidehttps_enabled(): mixed
```












***

### get_domain



```php
private get_domain(): mixed
```












***

### get_product_count



```php
private get_product_count(): mixed
```












***

### get_product_configuration_url



```php
public get_product_configuration_url(): mixed
```












***

### get_shipping_configuration_url



```php
public get_shipping_configuration_url(): mixed
```












***

### get_tax_configuration_url



```php
public get_tax_configuration_url(): mixed
```












***

### get_payment_configuration_url



```php
public get_payment_configuration_url(): mixed
```












***

### get_checkout_setup_documentation_url



```php
public get_checkout_setup_documentation_url(): mixed
```












***

### get_required_steps



```php
public get_required_steps(): mixed
```












***

### get_optional_steps



```php
public get_optional_steps(): mixed
```












***

### new_account



```php
public new_account(): mixed
```












***


***
> Automatically generated on 2024-12-10