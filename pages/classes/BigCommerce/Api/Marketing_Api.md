***

# Marketing_Api

Provides methods for interacting with marketing-related resources in BigCommerce,
including gift certificates.



* Full name: `\BigCommerce\Api\Marketing_Api`
* Parent class: [`\BigCommerce\Api\v2ApiAdapter`](./classes/BigCommerce/Api/v2ApiAdapter.md)




## Methods


### get_gift_certificate_by_code

Retrieve a gift certificate by its code.

```php
public get_gift_certificate_by_code(string $code): resource
```

Searches for a gift certificate matching the given code and returns the resource if found.
Throws an exception if no matching gift certificate is found.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$code` | **string** | The gift certificate code to search for. |


**Return Value:**

The gift certificate resource object.



**Throws:**
<p>If no gift certificate matches the provided code, or if the API call fails.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



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
