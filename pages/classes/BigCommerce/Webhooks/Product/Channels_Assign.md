***

# Channels_Assign





* Full name: `\BigCommerce\Webhooks\Product\Channels_Assign`
* Parent class: [`\BigCommerce\Webhooks\Product\Channels_Manager`](./Channels_Manager.md)




## Methods


### handle_request



```php
public handle_request(mixed $product_id, mixed $channel_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **mixed** |  |
| `$channel_id` | **mixed** |  |





***

### handle_product_creation



```php
private handle_product_creation(\BigCommerce\Api\v3\Model\Product $product, \WP_Term $channel): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Api\v3\Model\Product** |  |
| `$channel` | **\WP_Term** |  |





***

### handle_product_update



```php
private handle_product_update(\BigCommerce\Post_Types\Product\Product $product, \WP_Term $channel): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Post_Types\Product\Product** |  |
| `$channel` | **\WP_Term** |  |





***


## Inherited methods


### __construct



```php
public __construct(\BigCommerce\Api\v3\Api\CatalogApi $catalog_api, \BigCommerce\Api\v3\Api\ChannelsApi $channels_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$catalog_api` | **\BigCommerce\Api\v3\Api\CatalogApi** |  |
| `$channels_api` | **\BigCommerce\Api\v3\Api\ChannelsApi** |  |





***

### get_channel



```php
protected get_channel(mixed $channel_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channel_id` | **mixed** |  |





***

### maybe_get_existing_product



```php
protected maybe_get_existing_product(mixed $product_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
