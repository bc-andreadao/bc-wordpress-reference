***

# Channel_Connector

Class Channel_Connector

Responsible for connecting the WordPress site with
a BigCommerce channel

* Full name: `\BigCommerce\Taxonomies\Channel\Channel_Connector`



## Properties


### channels



```php
private \BigCommerce\Api\v3\Api\ChannelsApi $channels
```






***

### store_api



```php
private \BigCommerce\Api\Store_Api $store_api
```






***

## Methods


### __construct



```php
public __construct(\BigCommerce\Api\v3\Api\ChannelsApi $channels_api, \BigCommerce\Api\Store_Api $store_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channels_api` | **\BigCommerce\Api\v3\Api\ChannelsApi** |  |
| `$store_api` | **\BigCommerce\Api\Store_Api** |  |





***

### create_first_channel



```php
public create_first_channel(): mixed
```












***

### create_channel

Create a new Channel on the BigCommerce store

```php
private create_channel(string $name): int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$name` | **string** |  |


**Return Value:**

The ID of the WordPress term connected to that channel ID




***

### handle_connect_request

Handle a request to connect a new channel during onboarding

```php
public handle_connect_request(string|int $value): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **string&#124;int** |  |





***

### handle_create_request



```php
public handle_create_request(string|int $value): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **string&#124;int** |  |





***

### prevent_store_url_changes

Once connected to a channel, the merchant should not be able to edit the store
URL from the API credentials settings.

```php
public prevent_store_url_changes(bool|string $disabled_message): bool|string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$disabled_message` | **bool&#124;string** |  |





***


***
> Automatically generated on 2024-12-10