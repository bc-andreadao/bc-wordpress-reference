***

# Payments_Api

Provides methods for interacting with the Payments API in BigCommerce.

Includes functionality to retrieve payment methods and count them with optional filters.

* Full name: `\BigCommerce\Api\Payments_Api`
* Parent class: [`\BigCommerce\Api\v2ApiAdapter`](./v2ApiAdapter.md)




## Methods


### get_payment_methods_count

Retrieve the count of available payment methods.

```php
public get_payment_methods_count(bool $include_test_mode = false): int|bool
```

This method counts payment methods returned from the `/payments/methods` endpoint.
It includes a workaround for inconsistent data types in the API response.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$include_test_mode` | **bool** | Whether to include methods in test mode in the count.<br />Defaults to `false`, which excludes test mode methods. |


**Return Value:**

The number of payment methods, or `false` if the API response is empty or invalid.




***

### get_payment_methods

Retrieve all available payment methods.

```php
public get_payment_methods(): array
```

This method fetches the collection of payment methods from the `/payments/methods` endpoint.







**Return Value:**

An array of payment method resources.




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

- [`BadMethodCallException`](../../BadMethodCallException.md)



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
> Automatically generated on 2024-12-10
