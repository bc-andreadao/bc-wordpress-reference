***

# Purchase_Gift_Certificate_Handler

Handles the submission and processing of gift certificate purchase forms.



* Full name: `\BigCommerce\Forms\Purchase_Gift_Certificate_Handler`
* This class implements:
[`\BigCommerce\Forms\Form_Handler`](./Form_Handler.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;gift-purchase&#039;|

## Properties


### minimum

Minimum amount for a gift certificate.

```php
private float $minimum
```






***

### maximum

Maximum amount for a gift certificate.

```php
private float $maximum
```






***

### api

The CartApi instance used to interact with the cart and perform cart-related operations.

```php
private \BigCommerce\Api\v3\Api\CartApi $api
```






***

## Methods


### __construct

Purchase_Gift_Certificate_Handler constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CartApi $api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\v3\Api\CartApi** | The Cart API instance. |





***

### handle_request

Handle the gift certificate purchase request.

```php
public handle_request(array $submission): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** | The submitted form data. |





***

### should_handle_request



```php
private should_handle_request(mixed $submission): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **mixed** |  |





***

### validate_submission



```php
private validate_submission(mixed $submission): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **mixed** |  |





***

### sanitize_amount



```php
private sanitize_amount(mixed $amount): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$amount` | **mixed** |  |





***

### get_certificate_data



```php
private get_certificate_data(mixed $submission): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
