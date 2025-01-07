***

# Channels_Currency_Update





* Full name: `\BigCommerce\Webhooks\Product\Channels_Currency_Update`




## Methods


### __construct



```php
public __construct(\BigCommerce\Api\v3\Api\CurrencyApi $api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\v3\Api\CurrencyApi** |  |





***

### handle_request



```php
public handle_request(int $channel_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channel_id` | **int** |  |





***

### get_channel_currency_assignment



```php
protected get_channel_currency_assignment(int $channel_id): \BigCommerce\Api\v3\Model\CurrencyAssignments|false
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channel_id` | **int** |  |





***

### get_channel



```php
protected get_channel(int $channel_id): false|int|string|\WP_Term
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channel_id` | **int** |  |





***


***
> Automatically generated on 2025-01-07
