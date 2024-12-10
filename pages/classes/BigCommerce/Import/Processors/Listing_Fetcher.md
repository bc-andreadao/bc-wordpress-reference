***

# Listing_Fetcher





* Full name: `\BigCommerce\Import\Processors\Listing_Fetcher`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./Import_Processor.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STATE_OPTION`|public| |&#039;bigcommerce_import_listing_id_fetcher_state&#039;|
|`PRODUCT_LISTING_MAP`|public| |&#039;bigcommerce_product_listing_map&#039;|

## Properties


### channels



```php
private \BigCommerce\Api\v3\Api\ChannelsApi $channels
```






***

### limit



```php
private int $limit
```






***

### channel_term



```php
private \WP_Term $channel_term
```






***

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

### extract_next_from_response



```php
private extract_next_from_response(\BigCommerce\Api\v3\Model\ListingCollectionResponse $response): int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$response` | **\BigCommerce\Api\v3\Model\ListingCollectionResponse** |  |


**Return Value:**

The value for the parameter to use for the next page of results




***

### get_next



```php
private get_next(): mixed
```












***

### set_next



```php
private set_next(mixed $next): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$next` | **mixed** |  |





***

### get_state



```php
private get_state(): mixed
```












***

### set_state



```php
private set_state(array $state): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$state` | **array** |  |





***

### clear_state



```php
private clear_state(): mixed
```












***

### state_option



```php
private state_option(): mixed
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

### clear_cache

Clear caches that may be storing the option

```php
private clear_cache(string $option): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |





***


***
> Automatically generated on 2024-12-10
