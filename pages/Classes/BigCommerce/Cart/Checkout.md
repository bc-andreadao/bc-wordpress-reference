***

# Checkout

Handles requests during checkout from the Buy Now button for products.



* Full name: `\BigCommerce\Cart\Checkout`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;checkout&#039;|


## Methods


### __construct

Constructor.

```php
public __construct(\BigCommerce\Api_Factory $api_factory): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api_factory` | **\BigCommerce\Api_Factory** | Factory for creating API clients. |





***

### handle_request

Handle the request for redirecting to checkout.

```php
public handle_request(string $cart_id, \BigCommerce\Api\v3\Api\CartApi $cart_api): void
```

This method processes a checkout request based on the provided cart ID and redirects the user
to the appropriate checkout page or URL. If the cart ID is missing or an error occurs,
an error is displayed to the user.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart_id` | **string** | The ID of the cart to check out. |
| `$cart_api` | **\BigCommerce\Api\v3\Api\CartApi** | The BigCommerce Cart API client. |





***


***
> Automatically generated on 2025-01-13
