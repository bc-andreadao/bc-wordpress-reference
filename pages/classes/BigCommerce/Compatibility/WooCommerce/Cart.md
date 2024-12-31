***

# Cart

This class handles the interaction between the WooCommerce cart and BigCommerce's cart API.

It retrieves cart information, including the cart subtotal, and maps it to a WooCommerce-compatible format.

* Full name: `\BigCommerce\Compatibility\WooCommerce\Cart`



## Properties


### cart_contents_count

The count of items in the cart.

```php
public int $cart_contents_count
```







***

## Methods


### __construct

Cart constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CartApi $bc_cart_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_cart_api` | **\BigCommerce\Api\v3\Api\CartApi** | The BigCommerce CartApi instance used to interact with the BigCommerce cart. |





***

### get_cart_subtotal

Get the subtotal for the current cart.

```php
public get_cart_subtotal(): string|int
```









**Return Value:**

The formatted subtotal of the cart or 0 if the cart amount is unavailable.




***


***
> Automatically generated on 2024-12-31
