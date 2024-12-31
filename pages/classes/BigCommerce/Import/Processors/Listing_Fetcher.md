***

# Listing_Fetcher





* Full name: `\BigCommerce\Import\Processors\Listing_Fetcher`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./classes/BigCommerce/Import/Processors/Import_Processor.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STATE_OPTION`|public| |&#039;bigcommerce_import_listing_id_fetcher_state&#039;|
|`PRODUCT_LISTING_MAP`|public| |&#039;bigcommerce_product_listing_map&#039;|


## Methods


### __construct

Listing_Fetcher constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\ChannelsApi $channels, \WP_Term $channel_term, int $limit = 100): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channels` | **\BigCommerce\Api\v3\Api\ChannelsApi** | The Channels API connection to use for the import |
| `$channel_term` | **\WP_Term** |  |
| `$limit` | **int** | Number of listing IDs to fetch per request |





***

### run



```php
public run(): mixed
```












***


## Inherited methods


### get_option



```php
protected get_option(string $option, bool $default = false): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |
| `$default` | **bool** |  |





***

### update_option



```php
protected update_option(string $option, mixed $value, bool $autoload = false): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |
| `$value` | **mixed** |  |
| `$autoload` | **bool** |  |





***

### add_option



```php
protected add_option(string $option, mixed $value, bool $autoload = false): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |
| `$value` | **mixed** |  |
| `$autoload` | **bool** |  |





***

### delete_option



```php
protected delete_option(string $option): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |





***


***
> Automatically generated on 2024-12-31
