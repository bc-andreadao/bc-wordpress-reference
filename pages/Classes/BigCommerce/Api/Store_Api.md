***

# Store_Api

Handle retrieving information about the store from APIv2.



* Full name: `\BigCommerce\Api\Store_Api`
* Parent class: [`\BigCommerce\Api\v2ApiAdapter`](./classes/BigCommerce/Api/v2ApiAdapter.md)




## Methods


### getCustomerLoginToken

Get customer login token by ID.

```php
public getCustomerLoginToken(int $id, string $redirectUrl = &#039;&#039;, string $requestIp = &#039;&#039;, int $channel_id): string
```

This method generates a JWT token to allow a customer to log in. The token can
be used to authenticate the customer in future API requests.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$id` | **int** | The ID of the customer. |
| `$redirectUrl` | **string** | Optional URL to redirect the customer after login. |
| `$requestIp` | **string** | Optional IP address of the requestor. |
| `$channel_id` | **int** | Optional channel ID for the customer login. |


**Return Value:**

The generated JWT login token.



**Throws:**
<p>If the client secret is missing or other errors occur.</p>

- [`Exception`](./classes/Exception.md)



***

### get_analytics_settings

Return the list of store analytics settings.

```php
public get_analytics_settings(): array
```

This method retrieves the store's analytics settings, such as tracking options.







**Return Value:**

The store's analytics settings.




***

### update_analytics_settings

Update store analytics setting by ID.

```php
public update_analytics_settings(int $id, array $settings): bool
```

This method updates the analytics settings for a given store using the provided
settings array.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$id` | **int** | The ID of the analytics setting to update. |
| `$settings` | **array** | The new settings for the store. |


**Return Value:**

True if the update was successful, false otherwise.




***

### get_sitewidehttps_enabled

Check if site-wide HTTPS option is enabled in BigCommerce.

```php
public get_sitewidehttps_enabled(): bool
```

This method checks if the site-wide HTTPS option is enabled for the store.







**Return Value:**

True if HTTPS is enabled, false otherwise.




***

### get_domain

Get store domain.

```php
public get_domain(): bool
```

This method retrieves the domain name associated with the store.







**Return Value:**

The domain name of the store if available, otherwise false.




***

### store_resource_exists

Check whether the provided resource exists.

```php
public store_resource_exists(mixed $resource, string $property): bool
```

This method checks if a specific property exists in a given resource.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$resource` | **mixed** | The resource object to check. |
| `$property` | **string** | The property name to check for. |


**Return Value:**

True if the property exists in the resource, false otherwise.




***

### get_store_resource

Get store resource.

```php
public get_store_resource(): false|resource
```

This method retrieves the store resource containing details about the store.







**Return Value:**

The store resource, or false if an error occurs.




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
