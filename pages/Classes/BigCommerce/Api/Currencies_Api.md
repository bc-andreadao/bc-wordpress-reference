***

# Currencies_Api

Handles retrieval of currencies from the BigCommerce v2 API.

Provides a method to fetch and process a collection of currencies,
returning their properties as an associative array.

* Full name: `\BigCommerce\Api\Currencies_Api`
* Parent class: [`\BigCommerce\Api\v2ApiAdapter`](./classes/BigCommerce/Api/v2ApiAdapter.md)




## Methods


### get_currencies

Retrieve the list of currencies from the BigCommerce API.

```php
public get_currencies(): array
```

Fetches currencies from the `/currencies` endpoint and processes
them into an array of associative arrays, each representing a currency
and its updateable fields.







**Return Value:**

An array of currencies, where each currency is represented
as an associative array of its properties.



**Throws:**
<p>Handles exceptions gracefully, returning an empty array
if the API call fails.</p>

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
> Automatically generated on 2025-01-14
