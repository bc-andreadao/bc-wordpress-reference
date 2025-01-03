***

# Webhooks_Api

Creates an adapter class for the BC v2 API webhook endpoint.

Provides methods for managing webhooks through the BigCommerce v2 API, including listing,
creating, deleting, and updating webhooks.

* Full name: `\BigCommerce\Api\Webhooks_Api`
* Parent class: [`\BigCommerce\Api\v2ApiAdapter`](./classes/BigCommerce/Api/v2ApiAdapter.md)




## Methods


### listWebhooks

List all webhooks.

```php
public listWebhooks(): mixed
```

Retrieves a list of all webhooks through the client class's `listWebhooks` method.







**Return Value:**

The list of webhooks.




***

### createWebhook

Create a new webhook.

```php
public createWebhook(mixed $object): mixed
```

Creates a new webhook by calling the client class's `createWebhook` method.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$object` | **mixed** | The webhook object to create. |


**Return Value:**

The result of the create operation.




***

### deleteWebhook

Delete a webhook by ID.

```php
public deleteWebhook(int $id): mixed
```

Deletes the specified webhook by calling the client class's `deleteWebhook` method.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$id` | **int** | The ID of the webhook to delete. |


**Return Value:**

The result of the delete operation.




***

### updateWebhook

Update an existing webhook.

```php
public updateWebhook(int $id, mixed $object): mixed
```

Updates the specified webhook by calling the client class's `updateWebhook` method.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$id` | **int** | The ID of the webhook to update. |
| `$object` | **mixed** | The updated webhook data. |


**Return Value:**

The result of the update operation.




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
