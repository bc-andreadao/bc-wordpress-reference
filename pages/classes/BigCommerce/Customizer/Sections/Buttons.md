***

# Buttons

A customizer section that handles button label settings for various BigCommerce buttons in the WordPress Customizer.



* Full name: `\BigCommerce\Customizer\Sections\Buttons`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public|string|&#039;bigcommerce_buttons&#039;|
|`ADD_TO_CART`|public|string|&#039;bigcommerce_add_to_cart_button_label&#039;|
|`PREORDER_TO_CART`|public|string|&#039;bigcommerce_preorder_add_to_cart_button_label&#039;|
|`BUY_NOW`|public|string|&#039;bigcommerce_buy_now_button_label&#039;|
|`PREORDER_NOW`|public|string|&#039;bigcommerce_preorder_now_button_label&#039;|
|`CHOOSE_OPTIONS`|public|string|&#039;bigcommerce_choose_options_button_label&#039;|
|`VIEW_PRODUCT`|public|string|&#039;bigcommerce_view_product_button_label&#039;|


## Methods


### register

Registers the buttons section and related controls in the WordPress Customizer.

```php
public register(\WP_Customize_Manager $wp_customize): void
```

This method adds the buttons section and sets up controls for various button labels,
such as "Add to Cart," "Buy Now," and others.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** | The WordPress Customizer manager instance. |





***

### add_to_cart



```php
private add_to_cart(\WP_Customize_Manager $wp_customize): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** |  |





***

### preorder_add_to_cart



```php
private preorder_add_to_cart(\WP_Customize_Manager $wp_customize): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** |  |





***

### buy_now



```php
private buy_now(\WP_Customize_Manager $wp_customize): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** |  |





***

### preorder_buy_now



```php
private preorder_buy_now(\WP_Customize_Manager $wp_customize): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** |  |





***

### choose_options



```php
private choose_options(\WP_Customize_Manager $wp_customize): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** |  |





***

### view_product



```php
private view_product(\WP_Customize_Manager $wp_customize): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** |  |





***


***
> Automatically generated on 2024-12-10
