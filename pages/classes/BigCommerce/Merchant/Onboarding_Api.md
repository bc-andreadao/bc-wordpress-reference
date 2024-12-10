***

# Onboarding_Api





* Full name: `\BigCommerce\Merchant\Onboarding_Api`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`AUTH_KEY`|public| |&#039;bigcommerce_oauth_broker_secret&#039;|
|`ACCOUNT_ID`|public| |&#039;bigcommerce_account_id&#039;|
|`STORE_ID`|public| |&#039;bigcommerce_store_id&#039;|

## Properties


### base_url



```php
private string $base_url
```






***

### timeout



```php
private $timeout
```






***

## Methods


### __construct



```php
public __construct(string $base_url): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$base_url` | **string** |  |





***

### create_account



```php
public create_account(\BigCommerce\Merchant\Models\Create_Account_Request $request): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\BigCommerce\Merchant\Models\Create_Account_Request** |  |





***

### connect_account



```php
public connect_account(mixed $store_id, \BigCommerce\Merchant\Models\Connect_Account_Request $request): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$store_id` | **mixed** |  |
| `$request` | **\BigCommerce\Merchant\Models\Connect_Account_Request** |  |





***

### status



```php
public status(mixed $store_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$store_id` | **mixed** |  |





***

### build_auth_token

Build the auth token to make an authenticated request to the connector API

```php
private build_auth_token(mixed $store_id): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$store_id` | **mixed** |  |


**Return Value:**

The auth token, a JWT




***

### installation_url

Get the URL to launch the app installation process with BigCommerce

```php
public installation_url(string $store_id): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$store_id` | **string** |  |





***

### customer_login_token



```php
public customer_login_token(string $store_id, string $customer_id, \BigCommerce\Merchant\Models\Customer_Login_Request $request): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$store_id` | **string** |  |
| `$customer_id` | **string** |  |
| `$request` | **\BigCommerce\Merchant\Models\Customer_Login_Request** |  |




**Throws:**

- [`RuntimeException`](../../RuntimeException.md)



***


***
> Automatically generated on 2024-12-10
