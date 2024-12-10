***

# Caching_Client

Implements a short-term caching mechanism around API requests to reduce redundant calls,
particularly useful for operations like cart handling. The cache is invalidated after
any write operation to ensure data consistency.



* Full name: `\BigCommerce\Api\Caching_Client`
* Parent class: [`\BigCommerce\Api\Base_Client`](./Base_Client.md)



## Properties


### cache_group

Cache group identifier for WordPress caching.

```php
private string $cache_group
```






***

### generation_key

Cache generation key for versioning.

```php
private string $generation_key
```






***

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

- [`ApiException`](./v3/ApiException.md)



***

### is_write_operation

Identify if the request will write data to the API

```php
private is_write_operation(string $resourcePath, string $method, array $queryParams, array $postData): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$resourcePath` | **string** |  |
| `$method` | **string** |  |
| `$queryParams` | **array** |  |
| `$postData` | **array** |  |





***

### get_ttl_for_request



```php
private get_ttl_for_request(string $resourcePath, string $method, array $queryParams, array $postData): int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$resourcePath` | **string** |  |
| `$method` | **string** |  |
| `$queryParams` | **array** |  |
| `$postData` | **array** |  |





***

### read_methods



```php
private read_methods(): array
```









**Return Value:**

A list of all read operations




***

### build_cache_key

Build a unique identifier for the request

```php
private build_cache_key(mixed $resourcePath, mixed $method, mixed $queryParams, mixed $postData, mixed $headerParams, mixed $responseType): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$resourcePath` | **mixed** |  |
| `$method` | **mixed** |  |
| `$queryParams` | **mixed** |  |
| `$postData` | **mixed** |  |
| `$headerParams` | **mixed** |  |
| `$responseType` | **mixed** |  |





***

### get_generation_key



```php
private get_generation_key(): string
```









**Return Value:**

The generation key for cache versioning




***

### update_generation_key



```php
private update_generation_key(): void
```









**Return Value:**

Update the generation key based on the current timestamp




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
> Automatically generated on 2024-12-10
