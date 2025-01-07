***

# Remove_Item

Handles the logic for removing an item from a customer's wishlist.

This class processes the request to remove a specific product from a wishlist.
It ensures that the provided wishlist and product IDs are valid, removes the item from the wishlist,
and returns a success or error message accordingly.

* Full name: `\BigCommerce\Accounts\Wishlists\Actions\Remove_Item`
* Parent class: [`\BigCommerce\Accounts\Wishlists\Actions\Wishlist_Action`](./classes/BigCommerce/Accounts/Wishlists/Actions/Wishlist_Action.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;remove-item&#039;|


## Methods


### handle_request

Handles the request to remove a product from a specific wishlist.

```php
public handle_request(array $args): void
```

This method validates the request, retrieves the wishlist and product details,
and removes the product from the wishlist if it exists. A success or failure message is returned
based on the result of the operation.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | The arguments from the request. |





***

### sanitize_request

Sanitizes and validates the request to remove an item from a wishlist.

```php
protected sanitize_request(array $args, array $submission): array
```

This method ensures the wishlist ID and product ID are valid, sanitizes the request data,
and verifies the nonce to prevent unauthorized requests. It returns the validated data or throws
an exception if the data is invalid.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | The arguments from the request. |
| `$submission` | **array** | The request data to be validated. |


**Return Value:**

The sanitized and validated request data.



**Throws:**
<p>If the wishlist ID or product ID is invalid, or if the nonce is incorrect.</p>

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
> Automatically generated on 2025-01-07
