***

# Buy_Now

Handles requests from the Buy Now button for products.

Extends the Add_To_Cart class to reuse functionality for adding products to the cart,
with special handling for redirecting the user to the checkout page.

* Full name: `\BigCommerce\Cart\Buy_Now`
* Parent class: [`\BigCommerce\Cart\Add_To_Cart`](./classes/BigCommerce/Cart/Add_To_Cart.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public| |&#039;buy&#039;|


## Methods


### handle_response

Handles the response after a product has been successfully added to the cart and the purchase process begins.

```php
protected handle_response(\BigCommerce\Api\v3\Model\Cart $response, \BigCommerce\Cart\Cart $cart, int $post_id, int $product_id, int $variant_id): void
```

Redirects the user to the appropriate checkout page, either embedded or external.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$response` | **\BigCommerce\Api\v3\Model\Cart** | The response from the API after adding the product to the cart. |
| `$cart` | **\BigCommerce\Cart\Cart** | The Cart object containing cart data and methods. |
| `$post_id` | **int** | The ID of the product being purchased. |
| `$product_id` | **int** | The ID of the product being purchased. |
| `$variant_id` | **int** | The ID of the selected variant. |





***

### handle_exception

Handles exceptions that occur during the purchase process.

```php
protected handle_exception(\BigCommerce\Api\v3\ApiException $e, \BigCommerce\Cart\Cart $cart): void
```

Displays a user-friendly error message based on the API exception.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$e` | **\BigCommerce\Api\v3\ApiException** | The API exception that occurred during the purchase process. |
| `$cart` | **\BigCommerce\Cart\Cart** | The Cart object containing cart data. |





***


## Inherited methods


### handle_request

Handles the request to add a product to the cart.

```php
public handle_request(int $post_id, \BigCommerce\Api\v3\Api\CartApi $cart_api): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** | The ID of the product post. |
| `$cart_api` | **\BigCommerce\Api\v3\Api\CartApi** | The CartApi instance to interact with the cart API. |





***

### handle_response

Handles the response from the API after attempting to add a product to the cart.

```php
protected handle_response(\BigCommerce\Api\v3\Model\Cart|null $response, \BigCommerce\Cart\Cart $cart, int $post_id, int $product_id, int $variant_id): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$response` | **\BigCommerce\Api\v3\Model\Cart&#124;null** | The response from the API. |
| `$cart` | **\BigCommerce\Cart\Cart** | The cart instance. |
| `$post_id` | **int** | The ID of the product post. |
| `$product_id` | **int** | The ID of the product in BigCommerce. |
| `$variant_id` | **int** | The variant ID for the product. |





***

### handle_exception

Handles exceptions thrown during the cart API process.

```php
protected handle_exception(\BigCommerce\Api\v3\ApiException $e, \BigCommerce\Cart\Cart $cart): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$e` | **\BigCommerce\Api\v3\ApiException** | The exception thrown during the API request. |
| `$cart` | **\BigCommerce\Cart\Cart** | The cart instance. |





***

### validate_request

Validates the request to ensure the product exists and is published.

```php
protected validate_request(int $post_id, array $submission): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** | The ID of the product post. |
| `$submission` | **array** | The form submission data. |


**Return Value:**

True if the request is valid, false otherwise.




***

### get_variant_id

Gets the product variant ID from the form submission.

```php
protected get_variant_id(\BigCommerce\Post_Types\Product\Product $product, array $submission): int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Post_Types\Product\Product** | The product object. |
| `$submission` | **array** | The form submission data. |


**Return Value:**

The variant ID.




***


***
> Automatically generated on 2025-01-07
