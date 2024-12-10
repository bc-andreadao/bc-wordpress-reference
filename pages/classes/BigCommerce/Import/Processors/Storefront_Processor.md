***

# Storefront_Processor





* Full name: `\BigCommerce\Import\Processors\Storefront_Processor`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STOREFRONT_NAME`|public| |&#039;bigcommerce_storefront_name&#039;|
|`STOREFRONT_ADDRESS`|public| |&#039;bigcommerce_storefront_address&#039;|
|`STOREFRONT_EMAIl`|public| |&#039;bigcommerce_storefront_email&#039;|
|`STOREFRONT_PHONE`|public| |&#039;bigcommerce_storefront_phone&#039;|
|`DOWN_FOR_MAINTENANCE`|public| |&#039;bigcommerce_down_for_maintenance_message&#039;|
|`PRE_LAUNCH_MESSAGE`|public| |&#039;bigcommerce_prelaunch_message&#039;|
|`PRE_LAUNCH_PASSWORD`|public| |&#039;bigcommerce_prelaunch_password&#039;|
|`SHOW_PRODUCT_PRICE`|public| |&#039;bigcommerce_storefront_show_product_price&#039;|
|`SHOW_PRODUCT_SKU`|public| |&#039;bigcommerce_storefront_show_product_sku&#039;|
|`SHOW_PRODUCT_WEIGHT`|public| |&#039;bigcommerce_storefront_show_product_weight&#039;|
|`SHOW_PRODUCT_BRAND`|public| |&#039;bigcommerce_storefront_show_product_brand&#039;|
|`SHOW_PRODUCT_SHIPPING`|public| |&#039;bigcommerce_storefront_show_product_shipping&#039;|
|`SHOW_PRODUCT_RATING`|public| |&#039;bigcommerce_storefront_show_product_rating&#039;|
|`SHOW_PRODUCT_ADD_TO_CART_LINK`|public| |&#039;bigcommerce_storefront_show_add_to_cart_link&#039;|
|`DEFAULT_PREORDER_MESSAGE`|public| |&#039;bigcommerce_storefront_default_preorder_message&#039;|
|`SHOW_BREADCRUMBS_PRODUCT_PAGE`|public| |&#039;bigcommerce_storefront_show_breadcrumbs_product_pages&#039;|
|`SHOW_ADD_TO_CART_QTY_BOX`|public| |&#039;bigcommerce_storefront_show_add_to_cart_qty_box&#039;|
|`SHOW_ADD_TO_WISHLIST`|public| |&#039;bigcommerce_storefront_show_add_to_wishlist&#039;|
|`HIDE_PRICE_FROM_GUESTS`|public| |&#039;bigcommerce_storefront_hide_price_from_guests&#039;|


## Methods


### __construct



```php
public __construct(\BigCommerce\Api\v3\Api\SettingsApi $api, \BigCommerce\Taxonomies\Channel\Connections $connections): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\v3\Api\SettingsApi** |  |
| `$connections` | **\BigCommerce\Taxonomies\Channel\Connections** |  |





***

### run



```php
public run(): mixed
```












***

### handle_products

Get and save storefront product settings
/stores/{store_hash}/v3/settings/storefront/product
https://developer.bigcommerce.com/api-reference/d4a004e640c74-get-storefront-product-settings

```php
public handle_products(int $term_id, int $channel_id): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term_id` | **int** |  |
| `$channel_id` | **int** |  |





***

### handle_status

Get and save storefront status settings
/stores/{store_hash}/v3/settings/storefront/status
https://developer.bigcommerce.com/api-reference/9c3e93feb6a21-get-storefront-status

```php
public handle_status(int $term_id, int $channel_id): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term_id` | **int** |  |
| `$channel_id` | **int** |  |





***

### handle_profile_settings

Get and store storefront profile settings
/stores/{store_hash}/v3/settings/storefront/profile
https://developer.bigcommerce.com/api-reference/ac86db39bc51e-get-store-profile-settings

```php
public handle_profile_settings(int $term_id, int $channel_id): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term_id` | **int** |  |
| `$channel_id` | **int** |  |





***

### handle_options



```php
protected handle_options(int $term_id, array $entries = []): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term_id` | **int** |  |
| `$entries` | **array** |  |





***


***
> Automatically generated on 2024-12-10
