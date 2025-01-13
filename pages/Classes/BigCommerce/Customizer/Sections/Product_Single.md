***

# Product_Single

Handles settings and constants related to the single product page in the BigCommerce integration.

It defines various constants used for customization of product display, such as meta descriptions, gallery settings, pricing, and more.

* Full name: `\BigCommerce\Customizer\Sections\Product_Single`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public|string|&#039;bigcommerce_product_single&#039;|
|`RELATED_COUNT`|public|string|&#039;bigcommerce_max_related_products&#039;|
|`DEFAULT_IMAGE`|public|string|&#039;bigcommerce_default_image_id&#039;|
|`PRICE_DISPLAY`|public|string|&#039;bigcommerce_default_price_display&#039;|
|`INVENTORY_DISPLAY`|public|string|&#039;bigcommerce_inventory_display&#039;|
|`VARIANTS_DISABLED`|public|string|&#039;bigcommerce_variants_disabled&#039;|
|`META_DESC_DISABLE`|public|string|&#039;bigcommerce_meta_description_disabled&#039;|
|`GALLERY_SIZE`|public|string|&#039;bigcommerce_gallery_image_size&#039;|
|`HEADLESS_IMAGE_SIZE`|public|string|&#039;bigcommerce_gallery_headless_image_size&#039;|
|`ENABLE_ZOOM`|public|string|&#039;bigcommerce_enable_zoom&#039;|
|`ENABLE_PRICE_NONCE`|public|string|&#039;bigcommerce_enable_price_nonce&#039;|
|`SIZE_DEFAULT`|public|string|&#039;default&#039;|
|`SIZE_LARGE`|public|string|&#039;large&#039;|
|`SIZE_ORIGINAL`|public|string|&#039;original&#039;|
|`SIZE_CDN_STD`|public|string|&#039;standard&#039;|
|`SIZE_CDN_THUMB`|public|string|&#039;thumbnail&#039;|


## Methods


### register

Registers all customization options under the product single section.

```php
public register(\WP_Customize_Manager $wp_customize): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** | The WordPress customizer instance. |





***

### meta_description

Adds the meta description display setting and control.

```php
protected meta_description(\WP_Customize_Manager $wp_customize): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** | Customizer manager instance. |





***

### pricing_nonce

Registers the pricing nonce field option setting and control.

```php
protected pricing_nonce(\WP_Customize_Manager $wp_customize): void
```

Only enabled when the headless flag is set.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** | Customizer manager instance. |





***


***
> Automatically generated on 2025-01-13
