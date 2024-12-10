***

# Channel_Initializer

Initializes a channel by linking it to the full product catalog.

This process involves checking for existing products, skipping already linked products,
retrieving product listings, and adding new products to the channel.
The class also manages pagination for large product catalogs, ensuring that products
are processed in batches based on the set limit.

* Full name: `\BigCommerce\Import\Processors\Channel_Initializer`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./Import_Processor.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STATE_OPTION`|public|string|&#039;bigcommerce_import_channel_init_state&#039;|

## Properties


### channels

The ChannelsApi instance used to interact with the BigCommerce Channels API.

```php
private \BigCommerce\Api\v3\Api\ChannelsApi $channels
```

This API allows for managing channel-specific product listings and other channel-related operations.




***

### catalog

The CatalogApi instance used to interact with the BigCommerce Catalog API.

```php
private \BigCommerce\Api\v3\Api\CatalogApi $catalog
```

This API allows for retrieving product details, variants, and managing the product catalog.




***

### limit

The maximum number of product IDs to fetch per request.

```php
private int $limit
```

This value is used to limit the number of products retrieved during product imports.




***

### channel_term

The WordPress term associated with the channel.

```php
private \WP_Term $channel_term
```

This term represents the channel in the WordPress taxonomy and is used for associating products with the specific channel.




***

## Methods


### __construct

Channel_Initializer constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\ChannelsApi $channels, \BigCommerce\Api\v3\Api\CatalogApi $catalog, \WP_Term $channel_term, int $limit = 100): mixed
```

Initializes the Channel_Initializer class with the given parameters.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channels` | **\BigCommerce\Api\v3\Api\ChannelsApi** | The API object for managing channels. |
| `$catalog` | **\BigCommerce\Api\v3\Api\CatalogApi** | The API object for managing the product catalog. |
| `$channel_term` | **\WP_Term** | The WordPress term representing the channel. |
| `$limit` | **int** | The number of products to process per request (default 100). |





***

### is_existing_product

Check if the product exists

```php
private is_existing_product(mixed $product, mixed $channel_id): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **mixed** |  |
| `$channel_id` | **mixed** |  |





***

### run

Executes the channel initialization process.

```php
public run(): mixed
```

This includes retrieving products, checking their status, and adding them to the channel.
Handles pagination for large product catalogs.










***

### get_page



```php
private get_page(): mixed
```












***

### set_page



```php
private set_page(mixed $page): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$page` | **mixed** |  |





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

### multichannel_sync_channel_listings



```php
private multichannel_sync_channel_listings(): mixed
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
