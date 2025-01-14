***

# Delete_Wishlist

Handles the logic for deleting a wishlist.

This class processes the request to delete a specific wishlist for a customer. It validates
the provided wishlist ID, deletes the wishlist, and redirects the user to the default wishlist page.
It also triggers success or error actions based on the outcome of the operation.

* Full name: `\BigCommerce\Accounts\Wishlists\Actions\Delete_Wishlist`
* Parent class: [`\BigCommerce\Accounts\Wishlists\Actions\Wishlist_Action`](./classes/BigCommerce/Accounts/Wishlists/Actions/Wishlist_Action.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;delete&#039;|


## Methods


### handle_request

Handles the request to delete a specific wishlist.

```php
public handle_request(array $args): void
```

This method validates the request, retrieves the wishlist using the provided ID, and
deletes the wishlist from the system. Upon successful deletion, the user is redirected
to the wishlist page with a success message. If an error occurs, an error message is triggered.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | The arguments from the request. |





***

### sanitize_request

Validates and sanitizes the request to delete a wishlist.

```php
protected sanitize_request(array $args, array $submission): array
```

This method processes the submission data, ensuring the wishlist ID is valid and sanitizing
the request for security. It throws exceptions for invalid or missing data and returns a sanitized
array of the request data.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | The arguments from the request. |
| `$submission` | **array** | The submission data from the request. |


**Return Value:**

The sanitized request data, including the wishlist ID.



**Throws:**
<p>If the request is missing required fields or contains invalid data.</p>

- [`InvalidArgumentException`](./classes/InvalidArgumentException.md)



***


## Inherited methods


### __construct

Wishlist_Action constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\WishlistsApi $wishlists): mixed
```

Initializes the action with the WishlistsApi instance, allowing the action to interact with the BigCommerce API
for wishlist management.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wishlists` | **\BigCommerce\Api\v3\Api\WishlistsApi** | The WishlistsApi instance used for wishlist operations. |





***

### handle_request

Handle the incoming request.

```php
public handle_request(mixed $args): void
```

This is an abstract method that must be implemented by subclasses to handle the specific request for a wishlist action
(e.g., create, update, delete). The method should process the request and return the appropriate response.


* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** | The arguments for the action request, typically including the wishlist ID and any necessary data. |





***

### sanitize_request

Sanitize and validate the request data.

```php
protected sanitize_request(array $args, array $submission): array
```

This is an abstract method that must be implemented by subclasses to sanitize and validate the request submission
before performing any operations on the wishlist.


* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | The arguments for the action request. |
| `$submission` | **array** | The submitted form data, typically from a POST request. |


**Return Value:**

Sanitized data to be used in the action handler.




***

### get_customer_wishlist

Get the wishlist for the customer.

```php
protected get_customer_wishlist(int $user_id, int $wishlist_id): \BigCommerce\Accounts\Wishlists\Wishlist
```

Fetches the wishlist for a given customer based on their user ID and wishlist ID. If the wishlist is not found or
does not belong to the customer, an exception is thrown.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$user_id` | **int** | The ID of the user (customer). |
| `$wishlist_id` | **int** | The ID of the wishlist to retrieve. |


**Return Value:**

The customer's wishlist.



**Throws:**
<p>If the wishlist cannot be found or accessed.</p>

- [`RuntimeException`](./classes/RuntimeException.md)
<p>If the wishlist does not belong to the customer.</p>

- [`InvalidArgumentException`](./classes/InvalidArgumentException.md)



***

### get_customer_id

Get the Customer ID for the user.

```php
protected get_customer_id(int $user_id): int
```

Retrieves the customer ID associated with the given user ID.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$user_id` | **int** | The ID of the user (customer). |


**Return Value:**

The customer ID associated with the user.




***


***
> Automatically generated on 2025-01-14
