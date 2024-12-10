***

# Registration_Handler

Handles user registration requests and form submissions for account creation.



* Full name: `\BigCommerce\Forms\Registration_Handler`
* This class implements:
[`\BigCommerce\Forms\Form_Handler`](./Form_Handler.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;register-account&#039;|

## Properties


### spam_checker



```php
private \BigCommerce\Compatibility\Spam_Checker $spam_checker
```






***

### login



```php
private \BigCommerce\Accounts\Login $login
```






***

## Methods


### __construct

Constructor for the Registration_Handler class.

```php
public __construct(\BigCommerce\Compatibility\Spam_Checker $spam_checker, \BigCommerce\Accounts\Login $login): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$spam_checker` | **\BigCommerce\Compatibility\Spam_Checker** | Instance for checking spam submissions. |
| `$login` | **\BigCommerce\Accounts\Login** | Instance for handling user login. |





***

### handle_request

Handles form submission for user registration.

```php
public handle_request(array $submission): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** | The form submission data. |





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

### is_email_free



```php
private is_email_free(mixed $email): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$email` | **mixed** |  |





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

### is_spam



```php
private is_spam(mixed $submission): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **mixed** |  |





***

### validate_password



```php
private validate_password(mixed $password): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$password` | **mixed** |  |





***

### get_profile



```php
private get_profile(mixed $submitted_profile): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submitted_profile` | **mixed** |  |





***

### get_address



```php
private get_address(mixed $submitted_address): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submitted_address` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
