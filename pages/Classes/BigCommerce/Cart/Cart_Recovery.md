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


***
> Automatically generated on 2025-01-14
