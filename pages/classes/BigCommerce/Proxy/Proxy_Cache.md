***

# Proxy_Cache

Proxy_Cache class



* Full name: `\BigCommerce\Proxy\Proxy_Cache`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CACHE_GROUP_NAMESPACE`|public| |&#039;bigcommerce_proxy&#039;|
|`PRODUCTS_PATH`|public| |&#039;/catalog/products&#039;|
|`CATEGORIES_PATH`|public| |&#039;/catalog/categories&#039;|
|`BRANDS_PATH`|public| |&#039;/catalog/brands&#039;|
|`VARIANTS_PATH`|public| |&#039;/catalog/variants&#039;|
|`SUMMARY_PATH`|public| |&#039;/catalog/summary&#039;|
|`CHANNELS_PATH`|public| |&#039;/channels&#039;|
|`CACHE_TTL`|public| |10 * MINUTE_IN_SECONDS|
|`GENERATION_KEY_LENGTH`|public| |5|


## Methods


### __construct

Proxy_Cache constructor.

```php
public __construct(array $config): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **array** | Configuration details. |





***

### get_request_route_path

Returns all parts of a REST route after the base.

```php
public get_request_route_path(\WP_REST_Request $request): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Request object. |


**Return Value:**

The request path.




***

### get_generation

Provides a generation key for a cache group.

```php
public get_generation(string $cache_group): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cache_group` | **string** | Cache group name. |


**Return Value:**

Cache generation key.




***

### get_cache_key

Build a cache key from request args.

```php
public get_cache_key(\WP_REST_Request $request, string $cache_group): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP_REST_Request** | Request instance. |
| `$cache_group` | **string** | Cache group name. |


**Return Value:**

Cache key.




***

### get_cache_group_name

Returns a cache group name for a given REST request.

```php
public get_cache_group_name(string $route = null): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$route` | **string** | REST request route. |


**Return Value:**

Cache group name or an empty string if no cache group applies.




***

### handle_result

Caches responses from the BigCommerce API.

```php
public handle_result(mixed $result, \WP_REST_Request $request): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$result` | **mixed** | Results returned by the BigCommerce API. |
| `$request` | **\WP_REST_Request** | REST request. |





***

### cache_result

Caches data.

```php
public cache_result(mixed $data, string $cache_key, string $cache_group): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **mixed** | Data to cache. |
| `$cache_key` | **string** | Cache key. |
| `$cache_group` | **string** | Cache group name. |





***

### get_result

Fetch results from cache if $results are empty.

```php
public get_result(mixed $result, \WP_REST_Request $request): bool|mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$result` | **mixed** | Proxy results (This should be empty unless results are provided by extension). |
| `$request` | **\WP_REST_Request** | Request instance. |


**Return Value:**

Result.




***

### get_data_from_cache

Gets cached data.

```php
public get_data_from_cache(string $cache_key, string $cache_group): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cache_key` | **string** | A hash built from the request URL. |
| `$cache_group` | **string** | The request&#039;s cache group. |


**Return Value:**

Data or false if unsuccessful.




***

### bust_cache_group

Deletes a transient cache group

```php
public bust_cache_group(string $cache_group): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cache_group` | **string** | Cache group name. |





***

### bust_product_cache

Busts cache data related to a product that has been updated.

```php
public bust_product_cache(int $product_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** | The BigCommerce product ID. |





***


***
> Automatically generated on 2024-12-13
