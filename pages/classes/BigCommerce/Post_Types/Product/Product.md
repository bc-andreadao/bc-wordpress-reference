***

# Product





* Full name: `\BigCommerce\Post_Types\Product\Product`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bigcommerce_product&#039;|
|`BIGCOMMERCE_ID`|public| |&#039;bigcommerce_id&#039;|
|`BRAND_TRANSIENT`|public| |&#039;bigcommerce_brand_transient&#039;|
|`LISTING_ID`|public| |&#039;bigcommerce_listing_id&#039;|
|`SKU`|public| |&#039;bigcommerce_sku&#039;|
|`SKU_NORMALIZED`|public| |&#039;bigcommerce_sku_normalized&#039;|
|`SOURCE_DATA_META_KEY`|public| |&#039;bigcommerce_source_data&#039;|
|`LISTING_DATA_META_KEY`|public| |&#039;bigcommerce_listing_data&#039;|
|`MODIFIER_DATA_META_KEY`|public| |&#039;bigcommerce_modifier_data&#039;|
|`OPTIONS_DATA_META_KEY`|public| |&#039;bigcommerce_options_data&#039;|
|`OPTIONS_DATA_TRANSIENT`|public| |&#039;bigcommerce_options_transient&#039;|
|`CUSTOM_FIELDS_META_KEY`|public| |&#039;bigcommerce_custom_fields&#039;|
|`REQUIRES_REFRESH_META_KEY`|public| |&#039;bigcommerce_force_refresh&#039;|
|`IMPORTER_VERSION_META_KEY`|public| |&#039;bigcommerce_importer_version&#039;|
|`DATA_HASH_META_KEY`|public| |&#039;bigcommerce_data_hash&#039;|
|`GALLERY_META_KEY`|public| |&#039;bigcommerce_gallery&#039;|
|`VARIANT_IMAGES_META_KEY`|public| |&#039;bigcommerce_variant_images&#039;|
|`RATING_META_KEY`|public| |&#039;bigcommerce_rating&#039;|
|`RATING_SUM_META_KEY`|public| |&#039;bigcommerce_review_rating_sum&#039;|
|`REVIEW_COUNT_META_KEY`|public| |&#039;bigcommerce_review_count&#039;|
|`REVIEWS_APPROVED_META_KEY`|public| |&#039;bigcommerce_approved_review_count&#039;|
|`REVIEW_CACHE`|public| |&#039;bigcommerce_reviews&#039;|
|`SALES_META_KEY`|public| |&#039;bigcommerce_sales&#039;|
|`PRICE_META_KEY`|public| |&#039;bigcommerce_calculated_price&#039;|
|`PRICE_RANGE_META_KEY`|public| |&#039;bigcommerce_price_range&#039;|
|`INVENTORY_META_KEY`|public| |&#039;bigcommerce_inventory_level&#039;|


## Methods


### __construct



```php
public __construct(mixed $post_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **mixed** |  |





***

### get_redirect_product_link



```php
public get_redirect_product_link(): mixed
```












***

### __get



```php
public __get(mixed $property): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$property` | **mixed** |  |





***

### is_headless



```php
public is_headless(): mixed
```












***

### get_property



```php
public get_property(mixed $property): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$property` | **mixed** |  |





***

### post_id



```php
public post_id(): mixed
```












***

### bc_id



```php
public bc_id(): mixed
```












***

### sku



```php
public sku(): mixed
```












***

### get_reviews_sum



```php
public get_reviews_sum(): mixed
```












***

### get_reviews_count



```php
public get_reviews_count(): mixed
```












***

### brand



```php
public brand(): mixed
```












***

### condition



```php
public condition(): mixed
```












***

### show_condition



```php
public show_condition(): mixed
```












***

### on_sale



```php
public on_sale(): mixed
```












***

### price_range



```php
public price_range(): mixed
```












***

### calculated_price_range



```php
public calculated_price_range(): mixed
```












***

### retail_price

Get the retail price (MSRP) of the product

```php
public retail_price(): string
```









**Return Value:**

The formatted currency string for the product's retail price




***

### get_product_options



```php
public get_product_options(): mixed
```












***

### options



```php
public options(): mixed
```












***

### get_source_data

Get the product source data cached for this product

```php
public get_source_data(): object
```












***

### get_listing_data

Get the channel listing data cached for this product

```php
public get_listing_data(): object
```












***

### has_options

Check if a product has options.

```php
public has_options(): bool
```












***

### modifiers



```php
public modifiers(): mixed
```












***

### update_source_data



```php
public update_source_data(mixed $data): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **mixed** |  |





***

### update_listing_data



```php
public update_listing_data(mixed $data): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **mixed** |  |





***

### update_modifier_data



```php
public update_modifier_data(mixed $data): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **mixed** |  |





***

### update_options_data



```php
public update_options_data(mixed $data): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **mixed** |  |





***

### update_custom_field_data



```php
public update_custom_field_data(mixed $data): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **mixed** |  |





***

### get_custom_fields

Get custom fields for this Product

```php
public get_custom_fields(): array[]
```









**Return Value:**

An array of associative arrays, with the properties:
- name: the name to display for the field
- value: the value to display for the field




***

### get_gallery_ids



```php
public get_gallery_ids(): int[]
```









**Return Value:**

WP post IDs of gallery images




***

### get_headless_featured_image



```php
public get_headless_featured_image(string $size = &#039;80&#039;): string|null
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$size` | **string** |  |





***

### get_thumb_from_cdn



```php
public static get_thumb_from_cdn(mixed $post_ID, mixed $format = &#039;html&#039;, mixed $size = &#039;80&#039;): mixed
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_ID` | **mixed** |  |
| `$format` | **mixed** |  |
| `$size` | **mixed** |  |





***

### youtube_videos

Get the list of YouTube videos associated with the product

```php
public youtube_videos(): array
```












***

### purchase_url



```php
public purchase_url(): mixed
```












***

### purchase_button



```php
public purchase_button(): mixed
```












***

### purchase_message



```php
public purchase_message(): mixed
```












***

### get_variant_sku

Get product variant SKU by variant ID. Returns empty string if variant ID is not provided or wrong

```php
public get_variant_sku(int $variant_id): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$variant_id` | **int** |  |





***

### get_selected_variant_id

Get selected variant id

```php
public get_selected_variant_id(): int
```












***

### get_inventory_level



```php
public get_inventory_level(mixed $variant_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$variant_id` | **mixed** |  |





***

### out_of_stock

Checks if a product is out of stock. If a variant ID
is given and the product uses variant-level inventory
tracking, then it will be checked against the specific
variant.

```php
public out_of_stock(int $variant_id): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$variant_id` | **int** |  |


**Return Value:**

If the product is out of stock




***

### availability

Get the availability for the product

```php
public availability(): string
```












***

### is_purchasable

Checks if a product can be purchased, considering
both the purchasability setting and inventory levels

```php
public is_purchasable(int $variant_id): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$variant_id` | **int** |  |


**Return Value:**

If the product is out of stock




***

### low_inventory



```php
public low_inventory(): bool
```









**Return Value:**

Whether the product is below the "low inventory" threshold




***

### related_products

Get a list of products related to this one

```php
public related_products(array $args = []): int[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | Additional args to pass to WP_Query |


**Return Value:**

The IDs of related products




***

### get_reviews

Get the reviews associated with this product

```php
public get_reviews(int $count = 12): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$count` | **int** | The number of reviews to return. Will not return more<br />than the number in the review cache. |


**Return Value:**

The most recent reviews cached for the product




***

### get_review_count

Get the total number of reviews for the product

```php
public get_review_count(): int
```












***

### get_channel_id

Get the channel ID associated with this post

```php
public get_channel_id(): int
```









**Return Value:**

The BigCommerce channel ID




***

### get_channel

Get the Channel term associated with this post

```php
public get_channel(): \WP_Term
```









**Return Value:**

The WordPress Channel term




***

### get_listing_id

Get the Listing ID associated with this post

```php
public get_listing_id(): int
```









**Return Value:**

The BigCommerce Listing ID




***

### by_product_id

Gets a BigCommerce Product ID and returns matching Product object

```php
public static by_product_id(int $product_id, \WP_Term|null $channel = null, array $query_args = []): \BigCommerce\Post_Types\Product\Product|array
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** |  |
| `$channel` | **\WP_Term&#124;null** |  |
| `$query_args` | **array** |  |





***

### by_product_sku

Gets a BigCommerce Product SKU and returns matching Product object

```php
public static by_product_sku(string $product_sku, \WP_Term|null $channel = null, array $query_args = []): \BigCommerce\Post_Types\Product\Product|array
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_sku` | **string** |  |
| `$channel` | **\WP_Term&#124;null** |  |
| `$query_args` | **array** |  |





***


## Inherited methods


### format_currency

Formats a numeric value as a currency string.

```php
protected format_currency(float $value, string $empty_value = &#039;&#039;): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **float** | The currency value to format. |
| `$empty_value` | **string** | The value to return if $value is empty. Pass `null` to format anyway. |


**Return Value:**

The formatted currency string or the empty value.




***


***
> Automatically generated on 2024-12-10
