***

# Channel_Updater





* Full name: `\BigCommerce\Webhooks\Product\Channel_Updater`
* Parent class: [`\BigCommerce\Webhooks\Product\Channels_Manager`](./classes/BigCommerce/Webhooks/Product/Channels_Manager.md)




## Methods


### handle_request



```php
public handle_request(mixed $channel_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channel_id` | **mixed** |  |





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
> Automatically generated on 2025-01-14
