***

# Shipping_Api

Handles API v2 requests for shipping data, including zones and shipping methods.

Provides methods to fetch available shipping zones, count shipping methods,
and retrieve shipping methods by zone.

* Full name: `\BigCommerce\Api\Shipping_Api`
* Parent class: [`\BigCommerce\Api\v2ApiAdapter`](./classes/BigCommerce/Api/v2ApiAdapter.md)




## Methods


### get_zones

Get shipping zones.

```php
public get_zones(): array
```

This method retrieves the list of shipping zones configured in the BigCommerce store.







**Return Value:**

An array of shipping zones.




***

### count_shipping_methods

Get the count of available shipping methods.

```php
public count_shipping_methods(): int|float
```

This method retrieves all shipping zones and counts the available shipping methods
for each zone. If any errors occur during the retrieval process, it returns 0.







**Return Value:**

The total count of shipping methods available across all zones.




***

### get_shipping_methods

Retrieve the list of available shipping methods by zone ID.

```php
public get_shipping_methods(int $zone_id): array
```

This method retrieves the list of shipping methods for a specific shipping zone.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$zone_id` | **int** | The ID of the shipping zone for which to retrieve methods. |


**Return Value:**

An array of shipping methods for the specified zone.




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
> Automatically generated on 2025-01-07
