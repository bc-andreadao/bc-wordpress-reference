***

# Api_Scopes_Validator

Validates the API scopes for several resources, ensuring that the correct permissions
are in place during the onboarding process. This includes validating scopes for
customers, orders, and payment methods.



* Full name: `\BigCommerce\Api\Api_Scopes_Validator`
* Parent class: [`\BigCommerce\Api\v2ApiAdapter`](./classes/BigCommerce/Api/v2ApiAdapter.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CUSTOMERS_RESOURCE`|public|string|&#039;/customers&#039;|
|`MARKETING_RESOURCE`|public|string|&#039;/gift_certificates&#039;|
|`ORDERS_RESOURCE`|public|string|&#039;/orders&#039;|
|`PAYMENT_METHODS_RESOURCE`|public|string|&#039;/payments/methods&#039;|


## Methods


### validate

Validates scopes for several API items to ensure that the necessary permissions
are in place during the onboarding process.

```php
public validate(): bool
```

This method checks the scopes for customers, orders, and payment methods and
throws an exception if any of them are invalid.







**Return Value:**

Returns true if all scopes are valid.



**Throws:**
<p>If any of the scopes are invalid.</p>

- [`Exception`](./classes/Exception.md)



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
> Automatically generated on 2024-12-13
