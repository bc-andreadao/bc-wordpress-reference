***

# Add_Item

Handles requests for adding items to a customer's wishlist.

This class processes a request to add a product to the wishlist, sanitizes the request data,
verifies its validity, adds the item, and then provides a success or error message accordingly.

* Full name: `\BigCommerce\Accounts\Wishlists\Actions\Add_Item`
* Parent class: [`\BigCommerce\Accounts\Wishlists\Actions\Wishlist_Action`](./classes/BigCommerce/Accounts/Wishlists/Actions/Wishlist_Action.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;add-item&#039;|


## Methods


### handle_request

Handles the request to add an item to the wishlist.

```php
public handle_request(array $args): void
```

This method sanitizes the incoming request, verifies the wishlist and product IDs,
and adds the item to the wishlist. If successful, a success message is triggered;
if an error occurs, an error message is returned.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | The arguments from the request. |





***

### sanitize_request

Cleans up and sanitizes the add item request.

```php
protected sanitize_request(array $args, array $submission): array
```

This method verifies the wishlist ID and product ID, checks the nonce for security,
and ensures all required fields are provided and valid.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | The arguments from the request. |
| `$submission` | **array** | The submission data from the request. |


**Return Value:**

The sanitized request data, including the wishlist and product IDs.



**Throws:**
<p>If the request is invalid or missing required data.</p>

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
> Automatically generated on 2024-12-31
