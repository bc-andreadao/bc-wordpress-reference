***

# Channels_Manager





* Full name: `\BigCommerce\Webhooks\Product\Channels_Manager`



## Properties


### catalog_api



```php
protected \BigCommerce\Api\v3\Api\CatalogApi $catalog_api
```







***

### channels_api



```php
protected \BigCommerce\Api\v3\Api\ChannelsApi $channels_api
```







***

## Methods


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
> Automatically generated on 2024-12-13
