***

# Requirements_Notice

Shows a notice if the required configuration for checkout is not complete



* Full name: `\BigCommerce\Checkout\Requirements_Notice`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`REFRESH`|public|string|&#039;bigcommerce_checkout_requirements_refresh&#039;|

## Properties


### status



```php
private \BigCommerce\Merchant\Setup_Status $status
```






***

## Methods


### __construct

Constructor to initialize the setup status.

```php
public __construct(\BigCommerce\Merchant\Setup_Status $status): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$status` | **\BigCommerce\Merchant\Setup_Status** | Instance of Setup_Status to manage the store&#039;s setup status. |





***

### check_requirements

Checks the BigCommerce API to verify that checkout requirements
have been met. Displays admin notices if requirements are not satisfied.

```php
public check_requirements(): void
```












***

### get_settings_dashboard_url



```php
private get_settings_dashboard_url(): mixed
```












***

### refresh_status

Admin post handler to refresh the checkout requirements status cache.

```php
public refresh_status(): void
```












***

### refresh_url

Get the URL to trigger a status cache refresh

```php
private refresh_url(string $redirect = &#039;&#039;): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$redirect` | **string** | Redirect destination after refreshing the status cache |





***

### filter_embedded_checkout

Disables embedded checkout if SSL is not supported.

```php
public filter_embedded_checkout(int|bool $option): int|bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **int&#124;bool** | Current option value. |


**Return Value:**

Modified option value.




***

### can_enable_embedded_checkout

Determines if embedded checkout can be enabled.

```php
public can_enable_embedded_checkout(): bool
```









**Return Value:**

True if SSL is supported, false otherwise.




***


***
> Automatically generated on 2024-12-10
