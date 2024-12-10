***

# Channel_Synchronizer

Class Channel_Synchronizer

Synchronizes channel data in the WP taxonomy with
channels available via the API

* Full name: `\BigCommerce\Taxonomies\Channel\Channel_Synchronizer`



## Properties


### channels_api



```php
private \BigCommerce\Api\v3\Api\ChannelsApi $channels_api
```






***

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

### fetch_channels_from_api



```php
private fetch_channels_from_api(): \BigCommerce\Api\v3\Model\Channel[]
```











**Throws:**

- [`ApiException`](../../Api/v3/ApiException.md)



***

### mark_orphan

A term does not have a corresponding channel in the
API response. We have no idea what this term is. It shouldn't
be here, and it was likely added by a 3rd-party plugin or
left over from a previous installation that wasn't cleaned up.

```php
private mark_orphan(\WP_Term $term): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term` | **\WP_Term** |  |





***

### update_term



```php
private update_term(\WP_Term $term, mixed $channel): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term` | **\WP_Term** |  |
| `$channel` | **mixed** |  |





***

### insert_term

Create a new WP term for a channel

```php
private insert_term(\ArrayAccess|array $channel): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channel` | **\ArrayAccess&#124;array** |  |





***

### update_channel_status_meta



```php
private update_channel_status_meta(int $term_id, string $status): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term_id` | **int** |  |
| `$status` | **string** |  |





***

### bulk_assign_primary_channel

When creating the term for the primary channel,
bulk assign it to any product that does not already
have a channel assigned. This is to migrate sites
that already have products in the DB before multi-
channel was supported.

```php
private bulk_assign_primary_channel(int $term_id): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term_id` | **int** |  |





***


***
> Automatically generated on 2024-12-10
