***

# Password_Reset

Class Password_Reset

Responsible for handling customer password reset and synchronization with BigCommerce.

* Full name: `\BigCommerce\Accounts\Password_Reset`




## Methods


### __construct

Password_Reset constructor.

```php
public __construct(\BigCommerce\Api\Customer_Api $customer_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customer_api` | **\BigCommerce\Api\Customer_Api** | The Customer_Api instance for interacting with BigCommerce&#039;s API. |





***

### sync_reset_password_with_bigcommerce

Syncs the password reset with BigCommerce when a user submits the reset password form on the front end.

```php
public sync_reset_password_with_bigcommerce(\WP_User $user, string $new_pass): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$user` | **\WP_User** | The WordPress user object. |
| `$new_pass` | **string** | The new user password. |





***

### sync_password_change_with_bigcommerce

Syncs the password change with BigCommerce when a user's password is updated from the admin.

```php
public sync_password_change_with_bigcommerce(int $user_id, \WP_User $old_user_data): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$user_id` | **int** | The user ID. |
| `$old_user_data` | **\WP_User** | The WP_User object containing user&#039;s data prior to update. |





***


***
> Automatically generated on 2025-01-03
