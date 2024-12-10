***

# Account_Status





* Full name: `\BigCommerce\Merchant\Account_Status`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STATUS_AJAX`|public| |&#039;bigcommerce_account_status&#039;|

## Properties


### onboarding



```php
private \BigCommerce\Merchant\Onboarding_Api $onboarding
```






***

## Methods


### __construct



```php
public __construct(\BigCommerce\Merchant\Onboarding_Api $onboarding_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$onboarding_api` | **\BigCommerce\Merchant\Onboarding_Api** |  |





***

### render_status_placeholder

Render the placeholder div with the JS data for account status ajax requests

```php
public render_status_placeholder(): void
```












***

### handle_account_status_request

Handle the ajax request to update the store status

```php
public handle_account_status_request(): void
```












***

### validate_ajax_nonce

Validate the nonce for an ajax status request

```php
private validate_ajax_nonce(array $request): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **array** |  |





***

### save_store_hash

Save the store's hash to the DB

```php
private save_store_hash(string $hash): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$hash` | **string** |  |





***

### save_auth_credentials

Save the client ID and auth token to the DB

```php
private save_auth_credentials(string $client_id, string $auth_token): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$client_id` | **string** |  |
| `$auth_token` | **string** |  |





***


***
> Automatically generated on 2024-12-10
