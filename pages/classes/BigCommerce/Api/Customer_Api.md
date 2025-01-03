***

# Customer_Api

Provides methods for interacting with BigCommerce customers via the v2 API.

Includes functionality for validating customer passwords and retrieving customer
information by email address.

* Full name: `\BigCommerce\Api\Customer_Api`
* Parent class: [`\BigCommerce\Api\v2ApiAdapter`](./classes/BigCommerce/Api/v2ApiAdapter.md)




## Methods


### validatePassword

Validate a customer's password.

```php
public validatePassword(int $customer_id, string $password): bool
```

Checks if the provided password matches the stored password for the given customer ID.
Throws an exception if the customer ID does not exist.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customer_id` | **int** | The ID of the customer to validate. |
| `$password` | **string** | The password to validate. |


**Return Value:**

True if the password is valid, false otherwise.



**Throws:**
<p>If the customer ID is not found.</p>

- [`InvalidArgumentException`](./classes/InvalidArgumentException.md)



***

### find_customer_id_by_email

Find the customer ID associated with a given email address.

```php
public find_customer_id_by_email(string $email): int
```

Searches for a customer by email and returns their ID. Returns 0 if no customer
is found or if an error occurs during the API request.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$email` | **string** | The email address to search for. |


**Return Value:**

The customer ID if found, or 0 if not found or on failure.




***


## Inherited methods


### __construct

Constructor

```php
public __construct(\BigCommerce\Api\Base_Client $apiClient): mixed
```

Initializes the API client instance to be used in making requests.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$apiClient` | **\BigCommerce\Api\Base_Client** | The API client to use. |





***

### __call

Magic method to call methods on the client class.

```php
public __call(string $method, array $args): mixed
```

Dynamically calls methods on the client class if available. Throws an exception if the method does not exist.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$method` | **string** | The method name to call. |
| `$args` | **array** | The arguments to pass to the method. |


**Return Value:**

The result of the method call.



**Throws:**
<p>If the method is not found.</p>

- [`BadMethodCallException`](./classes/BadMethodCallException.md)



***

### get_store_hash

Retrieve the store hash from the API client configuration.

```php
protected get_store_hash(): string
```

Extracts the store hash from the API client's configuration using the host URL.







**Return Value:**

The store hash.




***


***
> Automatically generated on 2025-01-03
