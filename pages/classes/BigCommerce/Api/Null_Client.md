***

# Null_Client

A placeholder API client that disables API calls.

This class is typically used when API configuration is missing or incomplete.

Attempts to make API calls using this client will throw an exception.

* Full name: `\BigCommerce\Api\Null_Client`
* Parent class: [`\BigCommerce\Api\Base_Client`](./classes/BigCommerce/Api/Base_Client.md)




## Methods


### callApi

Attempt to make an API call.

```php
public callApi(string $resourcePath, string $method, array $queryParams, array $postData, array $headerParams, string|null $responseType = null, string|null $endpointPath = null): mixed
```

This method always throws an exception because the client is configured to prevent API calls.
It is intended to signal that required API configuration settings are missing.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$resourcePath` | **string** | Path to the API method endpoint. |
| `$method` | **string** | HTTP method to use for the request (e.g., GET, POST). |
| `$queryParams` | **array** | Parameters to include in the query string of the URL. |
| `$postData` | **array** | Parameters to include in the body of the request. |
| `$headerParams` | **array** | Headers to include in the request. |
| `$responseType` | **string&#124;null** | The expected response type (optional). |
| `$endpointPath` | **string&#124;null** | The original endpoint path before parameter substitution (optional). |


**Return Value:**

This method does not return a value; it always throws an exception.



**Throws:**
<p>Always thrown with a message indicating missing settings.</p>

- [`ConfigurationRequiredException`](./classes/BigCommerce/Api/ConfigurationRequiredException.md)



***


## Inherited methods


### __construct

Constructor for the Base_Client class

```php
public __construct(\BigCommerce\Api\Configuration|null $config = null): mixed
```

Initializes the API client with the provided configuration. If no configuration
is provided, it will use the default configuration.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **\BigCommerce\Api\Configuration&#124;null** | The configuration for this ApiClient. |





***

### getConfig

Gets the configuration of the API client

```php
public getConfig(): \BigCommerce\Api\Configuration
```

Returns the configuration object used by the API client.







**Return Value:**

Returns the Configuration object used by this API client.




***


***
> Automatically generated on 2024-12-31
