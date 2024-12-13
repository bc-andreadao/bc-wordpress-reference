***

# Banners_Api

Class Banners_Api

Retrieves banner data from the Banners v2 API collection. This class allows you
to fetch banners and their associated details, such as name, content, location,
and visibility.

* Full name: `\BigCommerce\Api\Banners_Api`
* Parent class: [`\BigCommerce\Api\v2ApiAdapter`](./classes/BigCommerce/Api/v2ApiAdapter.md)




## Methods


### get_banners

Fetches a list of banners from the Banners v2 API.

```php
public get_banners(): array
```

This method retrieves the banners collection from the API and maps each banner
to a simplified array format containing its relevant data such as ID, name, content,
item ID, location, creation date, visibility, and more.







**Return Value:**

Returns an array of banners with the following keys:
- 'id' (int)
- 'name' (string)
- 'content' (string)
- 'page' (string)
- 'item_id' (int)
- 'location' (string)
- 'date_created' (int)
- 'date_type' (string)
- 'date_from' (int)
- 'date_to' (int)
- 'visible' (bool)




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
> Automatically generated on 2024-12-13
