***

# Customer

Handles customer-specific data and resources such as customer addresses, profiles, orders, and related functionalities.

This class interacts with the BigCommerce API to fetch and manage data for customers associated with WordPress users.

* Full name: `\BigCommerce\Accounts\Customer`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CUSTOMER_ID_META`|public|string|&#039;bigcommerce_customer_id&#039;|


## Methods


### __construct

Customer constructor.

```php
public __construct(int $wp_user_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_user_id` | **int** | The WordPress user ID associated with the customer. |





***

### get_addresses

Get customer addresses.

```php
public get_addresses(): array
```

Fetches all the addresses associated with the customer.







**Return Value:**

An array of addresses associated with the customer.




***

### delete_address

Delete a customer's address by address ID.

```php
public delete_address(int $address_id): bool
```

Deletes the address associated with the provided address ID for the customer.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$address_id` | **int** | The ID of the address to be deleted. |


**Return Value:**

Returns true if the address was successfully deleted, false otherwise.




***

### add_address

Add a new address for the customer.

```php
public add_address(array $address): bool
```

Adds a new address to the customer's account.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$address` | **array** | The address data to be added. |


**Return Value:**

Returns true if the address was successfully added, false otherwise.




***

### update_address

Update a customer's address by address ID.

```php
public update_address(int $address_id, array $address): bool
```

Updates an existing address based on the provided address ID.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$address_id` | **int** | The ID of the address to be updated. |
| `$address` | **array** | The updated address data. |


**Return Value:**

Returns true if the address was successfully updated, false otherwise.




***

### get_order_count

Get the number of orders for the customer.

```php
public get_order_count(): int
```

Returns the total count of orders placed by the customer.







**Return Value:**

The number of orders associated with the customer.




***

### get_orders

Get the most recent orders of the customer.

```php
public get_orders(int $page = 1, int $limit = 12): array
```

Returns a list of the most recent orders for the customer, each including at least one product.
Note that this function makes multiple API calls and should be optimized for scalability in the future.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$page` | **int** | The page number of results. |
| `$limit` | **int** | The number of results per page. |


**Return Value:**

A list of the most recent orders of the customer.




***

### get_order_details

Get detailed information for a specific customer order.

```php
public get_order_details(int $order_id): array|false
```

Fetches detailed information about the specified order, including products and shipping addresses.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$order_id` | **int** | The ID of the order to retrieve. |


**Return Value:**

An array of order details or false if the order is not found.




***

### get_profile

Get the profile data of the customer.

```php
public get_profile(): array
```

Returns the customer's profile information, including fields like name, email, and customer group.







**Return Value:**

An array of customer profile data.




***

### update_profile

Update the profile data of the customer.

```php
public update_profile(array $profile): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$profile` | **array** | The profile data to update. |


**Return Value:**

Returns true if the profile was successfully updated, false otherwise.




***

### get_customer_id

Get the customer ID linked to the current WordPress user.

```php
public get_customer_id(): int
```









**Return Value:**

The customer ID associated with the WordPress user.




***

### set_customer_id

Set the customer ID linked to the current WordPress user.

```php
public set_customer_id(int $customer_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customer_id` | **int** | The customer ID to link to the WordPress user. |





***

### get_group_id

Get the customer group ID assigned to the user.

```php
public get_group_id(): int|null
```









**Return Value:**

The group ID of the customer, or null if the user is a guest.




***

### get_guests_default_group

Get the default group for guest users.

```php
public get_guests_default_group(): array|null
```









**Return Value:**

An array of default customer group IDs for guests, or null if none are found.




***

### get_group

Get the customer group for the current customer.

```php
public get_group(): \BigCommerce\Accounts\Customer_Group
```









**Return Value:**

The customer group object associated with the customer.




***


***
> Automatically generated on 2025-01-03
