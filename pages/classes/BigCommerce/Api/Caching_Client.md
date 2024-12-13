***

# Caching_Client

Implements a short-term caching mechanism around API requests to reduce redundant calls,
particularly useful for operations like cart handling. The cache is invalidated after
any write operation to ensure data consistency.



* Full name: `\BigCommerce\Api\Caching_Client`
* Parent class: [`\BigCommerce\Api\Base_Client`](./classes/BigCommerce/Api/Base_Client.md)




## Methods


### callApi

Perform an API call, utilizing caching for read operations.

```php
public callApi(string $resourcePath, string $method, array $queryParams, array $postData, array $headerParams, string|null $responseType = null, string|null $endpointPath = null): array
```

If the operation is a write, the cache generation key is updated to invalidate previous cache.
For read operations, the cache is checked first before making an API request.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$resourcePath` | **string** | Path to the API endpoint. |
| `$method` | **string** | HTTP method (e.g., GET, POST). |
| `$queryParams` | **array** | Query parameters for the request. |
| `$postData` | **array** | Data to include in the POST body. |
| `$headerParams` | **array** | Headers to include in the request. |
| `$responseType` | **string&#124;null** | Expected response type (optional). |
| `$endpointPath` | **string&#124;null** | Endpoint path before parameter expansion (optional). |


**Return Value:**

Response data from the API or cache.



**Throws:**
<p>If a non-2xx response is received.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



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
> Automatically generated on 2024-12-13
