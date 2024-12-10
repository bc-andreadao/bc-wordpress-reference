***

# Channel_Sync

Class Channel_Sync

Synchronizes changes to the Product state with the BigCommerce Channel

* Full name: `\BigCommerce\Post_Types\Product\Channel_Sync`



## Properties


### channels



```php
private \BigCommerce\Api\v3\Api\ChannelsApi $channels
```






***

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

### get_listing_state



```php
private get_listing_state(int $post_id, \BigCommerce\Api\v3\Model\Listing $listing): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** |  |
| `$listing` | **\BigCommerce\Api\v3\Model\Listing** |  |





***

### get_listing_title



```php
private get_listing_title(mixed $post_id, \BigCommerce\Api\v3\Model\Listing $listing): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **mixed** |  |
| `$listing` | **\BigCommerce\Api\v3\Model\Listing** |  |





***

### get_listing_description



```php
private get_listing_description(mixed $post_id, \BigCommerce\Api\v3\Model\Listing $listing): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **mixed** |  |
| `$listing` | **\BigCommerce\Api\v3\Model\Listing** |  |





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
> Automatically generated on 2024-12-10
