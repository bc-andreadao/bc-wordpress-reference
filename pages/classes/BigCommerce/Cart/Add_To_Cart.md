***

# Add_To_Cart

Handles requests from the Add to Cart button for products



* Full name: `\BigCommerce\Cart\Add_To_Cart`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public| |&#039;cart&#039;|


## Methods


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
