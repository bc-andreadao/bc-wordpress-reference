***

# Routes

Class Routes

Responsible for setting the routes for the site
connected to a channel

* Full name: `\BigCommerce\Taxonomies\Channel\Routes`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`VERSION`|public| |5|


## Methods


### __construct



```php
public __construct(\BigCommerce\Api\v3\Api\SitesApi $sites_api, \BigCommerce\Api\v3\Api\ChannelsApi $channels_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$sites_api` | **\BigCommerce\Api\v3\Api\SitesApi** |  |
| `$channels_api` | **\BigCommerce\Api\v3\Api\ChannelsApi** |  |





***

### set_routes



```php
public set_routes(int $channel_id): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channel_id` | **int** |  |





***

### schedule_update_routes

Schedule a cron event to trigger asynchronous route updates

```php
public schedule_update_routes(): void
```












***

### update_routes



```php
public update_routes(): void
```









**Return Value:**

Set new routes whenever any of the route list element gets updated




***

### update_site_home



```php
public update_site_home(): void
```












***

### update_route_permalink



```php
public update_route_permalink(int $post_id, \WP_Post $new_post, \WP_Post $old_post): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** | Post ID. |
| `$new_post` | **\WP_Post** | The Post Object |
| `$old_post` | **\WP_Post** | The Previous Post Object |





***

### get_route_list



```php
protected get_route_list(): \BigCommerce\Api\v3\Model\Route[]
```









**Return Value:**

A list of routes for pages on this site




***

### maybe_update_routes



```php
public maybe_update_routes(): void
```












***

### diagnostic_data

Add site and route info to diagnostic info

```php
public diagnostic_data(array $data): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **array** |  |





***


***
> Automatically generated on 2025-01-14
