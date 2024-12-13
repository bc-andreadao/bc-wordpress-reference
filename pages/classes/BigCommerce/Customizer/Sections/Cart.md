***

# Cart

Handles the customization options for the Cart section in the WordPress Customizer.

Allows users to enable or disable the mini-cart, set the empty cart link destination,
and control the visibility of shipping info and coupon codes in the cart.

* Full name: `\BigCommerce\Customizer\Sections\Cart`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public|string|&#039;bigcommerce_cart&#039;|
|`ENABLE_MINI_CART`|public|string|&#039;bigcommerce_enable_mini_cart&#039;|
|`EMPTY_CART_LINK`|public|string|&#039;bigcommerce_empty_cart_link_destination&#039;|
|`EMPTY_CART_LINK_TEXT`|public|string|&#039;bigcommerce_empty_cart_link_destination_text&#039;|
|`LINK_HOME`|public|string|&#039;home&#039;|
|`LINK_CATALOG`|public|string|&#039;catalog&#039;|
|`ENABLE_SHIPPING_INFO`|public|string|&#039;bigcommerce_enable_shipping_info&#039;|
|`ENABLE_COUPON_CODE`|public|string|&#039;bigcommerce_enable_coupon_code&#039;|


## Methods


### register

Registers settings and controls for Cart customization.

```php
public register(\WP_Customize_Manager $wp_customize): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** | The WordPress Customizer manager instance. |





***


***
> Automatically generated on 2024-12-13
