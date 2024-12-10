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

## Properties


### sites



```php
private \BigCommerce\Api\v3\Api\SitesApi $sites
```






***

### channels



```php
private \BigCommerce\Api\v3\Api\ChannelsApi $channels
```






***

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

### get_active_channel_ids

Get the IDs of all active channels (primary or connected)

```php
private get_active_channel_ids(): int[]
```












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

### get_site_id



```php
private get_site_id(int $channel_id): int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channel_id` | **int** | The ID of a channel |


**Return Value:**

The ID of the site associated with the channel. 0 if none found.




***

### create_site



```php
private create_site(int $channel_id): int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channel_id` | **int** |  |


**Return Value:**

The ID of the site created. 0 if an error occurs.




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

### get_post_type_route

A simplified version of the logic in get_post_permalink()
to get a sample URL for a post type for use in a route

```php
private get_post_type_route(string $post_type): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_type` | **string** |  |





***

### get_taxonomy_route

A simplified version of the logic in get_term_link()
to get a sample URL for a taxonomy for use in a route

```php
private get_taxonomy_route(string $taxonomy): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$taxonomy` | **string** |  |





***

### update_route



```php
private update_route(int $site_id, \BigCommerce\Api\v3\Model\Route $route): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$site_id` | **int** |  |
| `$route` | **\BigCommerce\Api\v3\Model\Route** |  |





***

### find_matching_route

Find a route that matches the Type and Matching properties of the given route

```php
private find_matching_route(int $site_id, \BigCommerce\Api\v3\Model\Route $route): \BigCommerce\Api\v3\Model\Route|null
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$site_id` | **int** |  |
| `$route` | **\BigCommerce\Api\v3\Model\Route** |  |





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
> Automatically generated on 2024-12-10
