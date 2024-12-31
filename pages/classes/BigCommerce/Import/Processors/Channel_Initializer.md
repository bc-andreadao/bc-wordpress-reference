***

# Channel_Initializer

Initializes a channel by linking it to the full product catalog.

This process involves checking for existing products, skipping already linked products,
retrieving product listings, and adding new products to the channel.
The class also manages pagination for large product catalogs, ensuring that products
are processed in batches based on the set limit.

* Full name: `\BigCommerce\Import\Processors\Channel_Initializer`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./classes/BigCommerce/Import/Processors/Import_Processor.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STATE_OPTION`|public|string|&#039;bigcommerce_import_channel_init_state&#039;|


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

### run

Executes the channel initialization process.

```php
public run(): mixed
```

This includes retrieving products, checking their status, and adding them to the channel.
Handles pagination for large product catalogs.










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
