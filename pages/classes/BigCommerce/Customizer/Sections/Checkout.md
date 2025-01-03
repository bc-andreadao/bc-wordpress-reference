***

# Checkout

Handles the customization options for the Checkout section in the WordPress Customizer.

Allows users to modify the colors of the embedded checkout page including background, text,
link, and error colors.

* Full name: `\BigCommerce\Customizer\Sections\Checkout`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public|string|&#039;bigcommerce_checkout&#039;|
|`BACKGROUND_COLOR`|public|string|&#039;bigcommerce_checkout_background_color&#039;|
|`TEXT_COLOR`|public|string|&#039;bigcommerce_checkout_text_color&#039;|
|`LINK_COLOR`|public|string|&#039;bigcommerce_checkout_link_color&#039;|
|`ERROR_COLOR`|public|string|&#039;bigcommerce_checkout_error_color&#039;|
|`COLOR_BLACK`|public|string|&#039;#000000&#039;|
|`COLOR_WHITE`|public|string|&#039;#FFFFFF&#039;|
|`COLOR_BC_BLUE`|public|string|&#039;#5273f4&#039;|
|`COLOR_BC_RED`|public|string|&#039;#ed1f00&#039;|


## Methods


### register

Registers settings and controls for Checkout customization.

```php
public register(\WP_Customize_Manager $wp_customize): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** | The WordPress Customizer manager instance. |





***


***
> Automatically generated on 2025-01-03
