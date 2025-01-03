***

# Amp_Cart

Class Amp_Cart

Handles AMP-specific cart functionalities such as retrieving cart details,
generating checkout URLs, and managing cart-related redirects.

* Full name: `\BigCommerce\Amp\Amp_Cart`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CHECKOUT_REDIRECT_ACTION`|public|string|&#039;amp_checkout&#039;|


## Methods


### __construct

Class constructor.

```php
public __construct(string $proxy_base): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$proxy_base` | **string** | Base path of the proxy REST endpoints. |





***

### get_checkout_url

Provides a URL endpoint to handle AMP checkout.

```php
public get_checkout_url(int|null $cart_id = null): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart_id` | **int&#124;null** | Unused in this implementation. |


**Return Value:**

URL to the AMP checkout endpoint.




***

### get_cart_id

Retrieves the cart ID from the browser's cookie.

```php
public get_cart_id(): string|false
```

Checks if the cart functionality is enabled and retrieves the cart ID
from the cookie set by BigCommerce.







**Return Value:**

Cart ID if available, false otherwise.




***

### get_cart_url

Gets the URL of the designated cart page.

```php
public get_cart_url(): string
```

Determines the URL of the cart page based on the WordPress option
for the cart page ID. Falls back to the home URL if no cart page is set.







**Return Value:**

URL of the cart page.




***

### handle_redirect_request

Handles redirection to the checkout URL for the current cart.

```php
public handle_redirect_request(): void
```

Uses the cart ID to generate a checkout URL via the BigCommerce API.
If the checkout URL cannot be retrieved, redirects back to the cart page.










***


***
> Automatically generated on 2025-01-03
