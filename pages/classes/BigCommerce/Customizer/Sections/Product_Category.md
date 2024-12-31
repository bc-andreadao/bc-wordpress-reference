***

# Product_Category

Handles the customization of product category settings and controls.



* Full name: `\BigCommerce\Customizer\Sections\Product_Category`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public|string|&#039;bigcommerce_product_categories&#039;|
|`CHILD_ITEM_SHOW`|public|string|&#039;bigcommerce_show_child_items&#039;|
|`CATEGORIES_IS_VISIBLE`|public|string|&#039;bigcommerce_categories_is_visible&#039;|


## Methods


### register

Register Product Category customize section and related controls.

```php
public register(\WP_Customize_Manager $wp_customize): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** | The WordPress Customizer instance. |





***

### add_is_visible_control

Register radio box control for categories "is visible" flag.

```php
protected add_is_visible_control(\WP_Customize_Manager $wp_customize): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** | The WordPress Customizer instance. |





***

### add_sub_categories_control

Register controls for showing child items in the navigation menu.

```php
protected add_sub_categories_control(\WP_Customize_Manager $wp_customize): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** | The WordPress Customizer instance. |





***


***
> Automatically generated on 2024-12-31
