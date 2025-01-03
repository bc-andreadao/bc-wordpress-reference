***

# Register

Class Register

Handles customer creation and synchronization with BigCommerce.

* Full name: `\BigCommerce\Accounts\Register`




## Methods


### __construct

Register constructor.

```php
public __construct(\BigCommerce\Api_Factory $api_factory, \BigCommerce\Taxonomies\Channel\Connections $connections): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api_factory` | **\BigCommerce\Api_Factory** | The API factory for interacting with BigCommerce&#039;s API. |
| `$connections` | **\BigCommerce\Taxonomies\Channel\Connections** | The connections instance for managing channels. |





***

### maybe_create_new_customer

Checks if the customer exists on BigCommerce, creates a new customer if not,
and associates the customer with the primary channel.

```php
public maybe_create_new_customer(int $user_id, array $userdata): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$user_id` | **int** | The user ID. |
| `$userdata` | **array** | The user data array. |





***

### is_customer_mail_in_use

Checks if the customer email is already registered in BigCommerce.

```php
protected is_customer_mail_in_use(string $email): bool|int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$email` | **string** | The customer email to check. |


**Return Value:**

Returns the customer ID if found, or false if not found.




***

### register_new_customer

Creates a new customer using the V3 API and associates them with the primary channel.

```php
protected register_new_customer(int $user_id, array $userdata): int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$user_id` | **int** | The user ID. |
| `$userdata` | **array** | The user data array. |


**Return Value:**

Returns the customer ID if successful, or 0 if creation failed.




***


***
> Automatically generated on 2025-01-03
