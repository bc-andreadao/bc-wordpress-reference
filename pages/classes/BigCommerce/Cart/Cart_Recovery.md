***

# Cart_Recovery

The Cart_Recovery class is responsible for handling the recovery of abandoned carts.

It interacts with BigCommerce's API to retrieve and recover abandoned carts based on
a unique token provided in the request. It also manages the redirection process and
the setting of cookies for recovered carts, ensuring that the user is taken to the correct
cart page and that the abandoned cart is appropriately handled.

* Full name: `\BigCommerce\Cart\Cart_Recovery`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;recover-cart&#039;|

## Properties


### cart_api



```php
private \BigCommerce\Api\v3\Api\CartApi $cart_api
```






***

### api



```php
private \BigCommerce\Api\v3\Api\AbandonedCartApi $api
```






***

## Methods


### __construct

Cart_Recovery constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\AbandonedCartApi $api, \BigCommerce\Api\v3\Api\CartApi $cart): mixed
```

Initializes the Cart_Recovery class with the given AbandonedCartApi and CartApi instances.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\v3\Api\AbandonedCartApi** | An instance of the AbandonedCartApi to interact with the BigCommerce API for cart recovery. |
| `$cart` | **\BigCommerce\Api\v3\Api\CartApi** | An instance of the CartApi to interact with the BigCommerce API for cart-related actions. |





***

### handle_request

Handles the incoming request to recover an abandoned cart.

```php
public handle_request(): string
```

This function retrieves the token from the query parameters, validates it,
and then attempts to recover the abandoned cart using the BigCommerce API.
If the cart is recovered successfully, it sets a cookie with the abandoned
cart's ID and redirects the user to the cart page. If there is an error,
it handles the error and redirects to the appropriate page.







**Return Value:**

The URL of the cart page, either with the recovered cart or as a fallback.




***

### redirect_to_cart

Redirects the user to the cart page.

```php
private redirect_to_cart(int $cart_page_id): mixed
```

This function redirects the user to the specified cart page using the cart page ID.
It performs the redirection and stops the script execution.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart_page_id` | **int** | The ID of the cart page to redirect to. |





***

### set_abandoned_cart_cookie

Sets a cookie for the recovered abandoned cart.

```php
private set_abandoned_cart_cookie(int $abandoned_cart): mixed
```

This function creates a Cart object and sets the cart ID of the recovered abandoned cart
to associate the user's session with the cart they are recovering.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$abandoned_cart` | **int** | The ID of the abandoned cart to be recovered. |





***


***
> Automatically generated on 2024-12-10
