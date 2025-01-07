***

# Channel_Sync

Class Channel_Sync

Synchronizes changes to the Product state with the BigCommerce Channel

* Full name: `\BigCommerce\Post_Types\Product\Channel_Sync`




## Methods


### __construct



```php
public __construct(\BigCommerce\Api\v3\Api\ChannelsApi $channels): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channels` | **\BigCommerce\Api\v3\Api\ChannelsApi** |  |





***

### post_updated

Listen for updates to product posts to trigger an update
to the BigCommerce channel listing

```php
public post_updated(int $post_id, \WP_Post $post): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** |  |
| `$post` | **\WP_Post** |  |





***

### post_deleted

When a post is deleted, permanently mark it deleted in the channel

```php
public post_deleted(int $post_id): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** |  |





***


***
> Automatically generated on 2025-01-07
