***

# BaseGQL

Handles interactions with the BigCommerce GraphQL API, including token management, making authenticated requests, and handling store-related information.



* Full name: `\BigCommerce\GraphQL\BaseGQL`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`GQL_BASE`|public|string|&#039;https://store-%s-%s.mybigcommerce.com/graphql&#039;|
|`GQL_ACCEPT`|public|string|&#039;application/json&#039;|
|`TOKEN_EXPIRATION`|public|string|&#039;bigcommerce_gql_expire_at&#039;|
|`GQL_TOKEN`|public|string|&#039;bigcommerce_gql_token&#039;|
|`GQL_IMPERSONATION_TOKEN`|public|string|&#039;bigcommerce_gql_im_token&#039;|
|`GQL_BASE_URL`|public|string|&#039;https://api.bigcommerce.com/stores/%s/v3/storefront/api-token&#039;|
|`GQL_IMPERSONATION_URL`|public|string|&#039;https://api.bigcommerce.com/stores/%s/v3/storefront/api-token-customer-impersonation&#039;|

## Properties


### token



```php
protected string $token
```







***

### impersonation_token



```php
protected string $impersonation_token
```







***

### config



```php
protected \BigCommerce\Api\v3\Configuration $config
```







***

## Methods


### __construct

Constructor.

```php
public __construct(\BigCommerce\Api\v3\Configuration $config): mixed
```

Initializes the BaseGQL instance with the provided configuration and retrieves the tokens.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **\BigCommerce\Api\v3\Configuration** | The configuration object used for API requests. |





***

### get_channel_id

Retrieves the current channel ID from the site transient or connections.

```php
protected get_channel_id(): int
```









**Return Value:**

The channel ID.




***

### get_token

Retrieves the current GraphQL token, requesting a new one if necessary.

```php
protected get_token(): mixed
```









**Return Value:**

The current token.




***

### get_impersonation_token

Retrieves the current impersonation token, requesting a new one if necessary.

```php
protected get_impersonation_token(): mixed
```









**Return Value:**

The current impersonation token.




***

### request_im_token

Requests a new impersonation token from the API and stores it in a transient.

```php
protected request_im_token(): void
```












***

### request_token

Requests a new GraphQL token from the API and stores it in a transient.

```php
protected request_token(): void
```












***

### make_request

Makes a POST request to the GraphQL API with the provided data, headers, and URL.

```php
public make_request(mixed $data, array $headers = [], string $url = &#039;&#039;): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **mixed** | The data to send in the request body. |
| `$headers` | **array** | The headers for the request. |
| `$url` | **string** | The URL for the request. |


**Return Value:**

The parsed response data.



**Throws:**
<p>If the request fails or the response is invalid.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***

### parse_response

Parses the response from the GraphQL API.

```php
protected parse_response(array $result): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$result` | **array** | The raw response data. |


**Return Value:**

The parsed response data.



**Throws:**
<p>If the response is invalid.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***

### get_store_hash

Retrieves the store hash from the configuration host URL.

```php
protected get_store_hash(): string
```









**Return Value:**

The store hash.




***

### get_endpoint_url

Retrieves the endpoint URL for the GraphQL request.

```php
protected get_endpoint_url(): string
```









**Return Value:**

The full GraphQL endpoint URL.




***

### get_origin

Retrieves the origin (site URL) for the request.

```php
protected get_origin(): string
```









**Return Value:**

The origin URL.




***

### get_auth_bearer

Constructs the authorization bearer string for the request.

```php
protected get_auth_bearer(bool $impersonation = false): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$impersonation` | **bool** | Whether to use the impersonation token. |


**Return Value:**

The authorization header value.




***

### validate_token

Validates whether the current token is still valid and not expired.

```php
protected validate_token(): bool
```









**Return Value:**

Whether the token is valid.




***

### get_headers

Constructs the headers for the GraphQL request, including authorization.

```php
protected get_headers(bool $impersonation = false): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$impersonation` | **bool** | Whether to use the impersonation token. |


**Return Value:**

The request headers.




***


***
> Automatically generated on 2025-01-07
