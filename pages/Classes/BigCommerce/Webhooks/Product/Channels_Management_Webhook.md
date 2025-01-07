***

# Channels_Management_Webhook

Class Channels_Management_Webhook

Sets up the webhook that runs on channels changes.

* Full name: `\BigCommerce\Webhooks\Product\Channels_Management_Webhook`
* Parent class: [`\BigCommerce\Webhooks\Webhook`](./classes/BigCommerce/Webhooks/Webhook.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`SCOPE`|public| |&#039;store/channel/*&#039;|
|`CHANNEL_UPDATED_SCOPE`|public| |&#039;store/channel/updated&#039;|
|`CHANNEL_UPDATED_HOOK`|public| |&#039;bigcommerce/webhooks/channel_updated&#039;|
|`NAME`|public| |&#039;bigcommerce_channels&#039;|
|`PRODUCT_CATEGORY_CHANNEL_HOOK`|public| |&#039;bigcommerce/webhooks/product_category_channel&#039;|
|`PRODUCT_CHANNEL_HOOK`|public| |&#039;bigcommerce/webhooks/product_channel&#039;|
|`CHANNEL_CURRENCY_UPDATE_HOOK`|public| |&#039;bigcommerce/webhooks/channel_default_currency_updated&#039;|


## Methods


### trigger_action

Fires when a change is applied to channels

```php
public trigger_action(array $request): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **array** |  |





***

### handle_channels_webhooks_filters



```php
public handle_channels_webhooks_filters(array $request, string $scope, int $channel_id, string $action): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **array** |  |
| `$scope` | **string** |  |
| `$channel_id` | **int** |  |
| `$action` | **string** |  |





***


## Inherited methods


### __construct

Webhook constructor

```php
public __construct(\BigCommerce\Api\Webhooks_Api $api_client): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api_client` | **\BigCommerce\Api\Webhooks_Api** | The client for making requests. |





***

### get_name



```php
public get_name(): mixed
```












***

### get_auth_header

Returns the value of the auth header.

```php
public get_auth_header(): string|bool|null
```









**Return Value:**

The value, or false or null if filter_input fails.




***

### create

Sends a request to BigCommerce to create a webhook.

```php
public create(array $args): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | Request arguments. |


**Return Value:**

Webhook data or an error response on failure.




***

### is_webhook_exist

Check by destination and scope if webhook is already added to BigCommerce.

```php
public is_webhook_exist(): mixed|null
```

Returns the id of the webhook










***

### update

Sends a request to the BC API to update a webhook. Creates it if it doesn't exist.

```php
public update(): mixed
```












***

### update_webhook

Send API request to update the webhook data

```php
public update_webhook(mixed $id, mixed $data): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$id` | **mixed** |  |
| `$data` | **mixed** |  |





***

### destination



```php
public destination(): mixed
```












***

### scope



```php
public scope(): mixed
```












***

### delete

Deletes a webhook from the BigCommerce database.

```php
public delete(int $webhook_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$webhook_id` | **int** | The BC ID for the webhook entry. |





***

### validate

Validates an incoming request.

```php
public validate(array $request, string|bool|null $password = null): bool|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **array** | Request data. |
| `$password` | **string&#124;bool&#124;null** | The password to authenticate with. |


**Return Value:**

True on validation or a WP_Error if the request isn't valid.




***

### get_webhook_payload

Get JSON input submitted from BigCommerce.

```php
public get_webhook_payload(): array
```









**Return Value:**

JSON data converted to an array.




***

### receive

Handles a webhook request.

```php
public receive(): mixed
```












***

### trigger_action

Triggers an action based on the webhook type and the request payload

```php
protected trigger_action(array $request): void
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **array** |  |





***


***
> Automatically generated on 2025-01-07
