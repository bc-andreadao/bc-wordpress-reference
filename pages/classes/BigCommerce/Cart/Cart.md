***

# Cart

Handles cart operations such as adding line items, managing cookies, and interacting with the BigCommerce API.



* Full name: `\BigCommerce\Cart\Cart`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CART_COOKIE`|public|string|&#039;wp-bigcommerce_cart_id&#039;|
|`COUNT_COOKIE`|public|string|&#039;wp-bigcommerce_cart_item_count&#039;|


## Methods


### __construct

Cart constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CartApi $api): mixed
```

Initializes the Cart class with the given CartApi instance.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\v3\Api\CartApi** | The BigCommerce Cart API instance. |





***

### get_cart_id

Get the cart ID from the cookie.

```php
public get_cart_id(): string
```

Retrieves the cart ID from the cookie and applies any relevant filters.







**Return Value:**

The cart ID.




***

### set_cart_id

Set the cookie that contains the cart ID.

```php
public set_cart_id(string $cart_id): void
```

Sets a cookie with the given cart ID, applying filters to determine the cookie's lifetime.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart_id` | **string** | The cart ID to set in the cookie. |





***

### add_line_item

Add a line item to the cart.

```php
public add_line_item(int $product_id, array $options = [], int $quantity = 1, array $modifiers = []): \BigCommerce\Api\v3\Model\Cart
```

Adds a product to the cart with the specified options, quantity, and modifiers.
The function handles both options and modifiers and sends the data to BigCommerce.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** | The BigCommerce ID of the product. |
| `$options` | **array** | All options and modifiers for the line item. |
| `$quantity` | **int** | How many to add to the cart. |
| `$modifiers` | **array** | Deprecated in 1.7.0, all values should be passed in $options. |


**Return Value:**

The updated cart after adding the line item.



**Throws:**
<p>If an error occurs while interacting with the BigCommerce API.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***

### add_gift_certificate

Add a gift certificate to the cart.

```php
public add_gift_certificate(mixed $certificate): \BigCommerce\Api\v3\Model\Cart
```

Adds a gift certificate to the cart, sending the data to BigCommerce for processing.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$certificate` | **mixed** | The gift certificate data to be added to the cart. |


**Return Value:**

The updated cart after adding the gift certificate.



**Throws:**
<p>If an error occurs while interacting with the BigCommerce API.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***

### sanitize_cart_id

Sanitize the cart ID by ensuring the cart still exists

```php
public sanitize_cart_id(string $cart_id): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart_id` | **string** | The cart ID to sanitize |


**Return Value:**

The sanitized cart ID or an empty string if not valid




***

### get_cart_url

Get the URL to the cart page

```php
public get_cart_url(): string
```









**Return Value:**

The URL to the cart page




***

### get_checkout_url

Get the checkout URL for the given cart ID

```php
public get_checkout_url(string $cart_id): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart_id` | **string** | The ID of the user&#039;s cart. Defaults to the ID found in the cart cookie |


**Return Value:**

The URL for checking out with the given cart




***

### get_embedded_checkout_url

Get the embedded checkout URL for the given cart ID

```php
public get_embedded_checkout_url(string $cart_id): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart_id` | **string** | The ID of the user&#039;s cart. Defaults to the ID found in the cart cookie |


**Return Value:**

The URL for the embedded checkout with the given cart




***

### delete_cart

Delete the cart by its ID

```php
public delete_cart(): void
```












***


***
> Automatically generated on 2025-01-03
