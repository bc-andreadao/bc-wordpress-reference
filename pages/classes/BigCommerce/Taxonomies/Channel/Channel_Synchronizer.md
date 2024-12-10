***

# Channel_Synchronizer

Class Channel_Synchronizer

Synchronizes channel data in the WP taxonomy with
channels available via the API

* Full name: `\BigCommerce\Taxonomies\Channel\Channel_Synchronizer`




## Methods


### __construct



```php
public __construct(\BigCommerce\Api\v3\Api\ChannelsApi $channels_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channels_api` | **\BigCommerce\Api\v3\Api\ChannelsApi** |  |





***

### initial_sync

Run an initial sync if channels have not been previously imported

```php
public initial_sync(): void
```












***

### handle_name_change

If a Channel name is changed, push the change up to the API

```php
public handle_name_change(int $term_id): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term_id` | **int** |  |





***

### sync



```php
public sync(): void
```












***


***
> Automatically generated on 2024-12-10
