***

# Create_Account





* Full name: `\BigCommerce\Merchant\Create_Account`



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

### request_account



```php
public request_account(array $submission, \WP_Error $errors): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** | The data submitted to the new account form |
| `$errors` | **\WP_Error** | Error object to collect any errors that occur |





***

### handle_error_response

Add errors from the response to the error accumulator

```php
private handle_error_response(array $response, \WP_Error $errors): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$response` | **array** |  |
| `$errors` | **\WP_Error** |  |





***


***
> Automatically generated on 2024-12-10