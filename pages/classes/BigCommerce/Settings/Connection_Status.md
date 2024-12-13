***

# Connection_Status





* Full name: `\BigCommerce\Settings\Connection_Status`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STATUS_CACHE`|public| |&#039;bigcommerce_connection_status&#039;|
|`STATUS_CACHE_TTL`|public| |60|


## Methods


### __construct

Connection_Status constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CatalogApi $client, bool $configuration_status): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$client` | **\BigCommerce\Api\v3\Api\CatalogApi** |  |
| `$configuration_status` | **bool** | Whether API configuration settings are fully in place |





***

### register_field



```php
public register_field(): mixed
```












***

### render_status



```php
public render_status(): mixed
```












***

### credentials_required_notice

Display a notice if all required credentials are not set.

```php
public credentials_required_notice(\BigCommerce\Settings\Screens\Abstract_Screen $target_screen, string[] $excluded_screens = []): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$target_screen` | **\BigCommerce\Settings\Screens\Abstract_Screen** | Settings screen the link will point to |
| `$excluded_screens` | **string[]** | Settings screen IDs that should not show the notice |





***

### flush_status_cache



```php
public flush_status_cache(): void
```












***


***
> Automatically generated on 2024-12-13
