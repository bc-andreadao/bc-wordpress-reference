***

# Status

Class Status

Handle webhook status data. Provides diagnostic data and handle webhook subscription

* Full name: `\BigCommerce\Webhooks\Status`



## Properties


### hooks



```php
private \BigCommerce\Webhooks\Webhook[] $hooks
```






***

### api



```php
private \BigCommerce\Api\Webhooks_Api $api
```






***

## Methods


### __construct

Status constructor.

```php
public __construct(\BigCommerce\Webhooks\Webhook[] $hooks, \BigCommerce\Api\Webhooks_Api $api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$hooks` | **\BigCommerce\Webhooks\Webhook[]** |  |
| `$api` | **\BigCommerce\Api\Webhooks_Api** |  |





***

### diagnostic_data

Return a list of webhooks for current BC store

```php
public diagnostic_data(array $data): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **array** |  |





***

### update_option



```php
public update_option(mixed $old_value, mixed $new_value, mixed $option_name): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$old_value` | **mixed** |  |
| `$new_value` | **mixed** |  |
| `$option_name` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10