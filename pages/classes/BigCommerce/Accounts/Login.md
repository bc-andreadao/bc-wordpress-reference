***

# Login

Handles the login and lost password logic for the BigCommerce account integration with WordPress.

This class connects WordPress users to BigCommerce customers, processes customer login, and provides the necessary functionality for user management.

* Full name: `\BigCommerce\Accounts\Login`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CUSTOMER_ID_META`|public| |&#039;bigcommerce_customer_id&#039;|


## Methods


### __construct

Login constructor.

```php
public __construct(\BigCommerce\Api_Factory $api_factory): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api_factory` | **\BigCommerce\Api_Factory** | The API factory to be used for creating API instances. |





***

### connect_customer_id

Connect the user to a BigCommerce account, if it exists

```php
public connect_customer_id(string $username, \WP_User $user): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$username` | **string** |  |
| `$user` | **\WP_User** |  |





***

### login_url

Filters the login URL to point to the front-end login page

```php
public login_url(string $login_url, string $redirect, bool $force_reauth): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$login_url` | **string** | The login URL. Not HTML-encoded. |
| `$redirect` | **string** | The path to redirect to on login, if supplied. |
| `$force_reauth` | **bool** | Whether to force reauthorization, even if a cookie is present. |





***

### login_error_handler

Handle errors from the login form, redirecting back
to the front-end login page.

```php
public login_error_handler(\WP_Error $errors, string $redirect): \WP_Error
```

Note that is hooked in on a filter, not an action,
since the latter was not available.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$errors` | **\WP_Error** |  |
| `$redirect` | **string** |  |





***

### lostpassword_url

Get lost password url

```php
public lostpassword_url(string $login_url, string $redirect): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$login_url` | **string** |  |
| `$redirect` | **string** |  |





***

### before_reset_password_email

If a user exists only on BC, try to sync before reset password email is sent.

```php
public before_reset_password_email(\WP_User|false $user_data, \WP_Error $errors): \WP_User|false
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$user_data` | **\WP_User&#124;false** | WP_User object if found, false if the user does not exist. |
| `$errors` | **\WP_Error** | A WP_Error object containing any errors generated<br />by using invalid credentials. |





***

### lostpassword_error_handler



```php
public lostpassword_error_handler(\WP_Error $error): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$error` | **\WP_Error** |  |





***

### register_url

Handle registration url

```php
public register_url(string $url): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$url` | **string** |  |





***

### redirect_account_pages_to_auth

Redirect all account pages to the login screen
for unauthenticated users.

```php
public redirect_account_pages_to_auth(): void
```












***

### redirect_auth_pages_to_account

Redirect the login/registration pages to the
account page for logged in users.

```php
public redirect_auth_pages_to_account(): void
```












***

### authenticate_new_user

If a user logs in with credentials for a user in BigCommerce
that do not match a user in WordPress, create a user account
and log the user in.

```php
public authenticate_new_user(\WP_User|\WP_Error|null $user, string $username, string $password): \WP_User|\WP_Error|null
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$user` | **\WP_User&#124;\WP_Error&#124;null** |  |
| `$username` | **string** |  |
| `$password` | **string** |  |





***

### check_password_for_linked_accounts

Validate password for accounts

```php
public check_password_for_linked_accounts(bool $match, string $password, string $hash, string|int $user_id): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$match` | **bool** | Whether the passwords match. |
| `$password` | **string** | The plaintext password. |
| `$hash` | **string** | The hashed password. |
| `$user_id` | **string&#124;int** | User ID. Can be empty. |





***


***
> Automatically generated on 2024-12-10
