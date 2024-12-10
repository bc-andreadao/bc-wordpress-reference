***

# Cart_Mapper

Maps a cart from the API to a standard format usable by the
REST API and other templates.



* Full name: `\BigCommerce\Cart\Cart_Mapper`



## Properties


### cart



```php
private \BigCommerce\Api\v3\Model\Cart $cart
```






***

### channel



```php
private \WP_Term $channel
```






***

## Methods


### __construct

Cart_Mapper constructor.

```php
public __construct(\BigCommerce\Api\v3\Model\Cart $cart): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart` | **\BigCommerce\Api\v3\Model\Cart** | The cart to map. |





***

### map

Maps the cart data into a format for API and template usage.

```php
public map(): array
```









**Return Value:**

Mapped cart data.




***

### map_coupon_data



```php
private map_coupon_data(array $coupons): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$coupons` | **array** |  |





***

### get_coupons_discount_amount



```php
private get_coupons_discount_amount(array $coupons): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$coupons` | **array** |  |





***

### cart_items



```php
private cart_items(): mixed
```












***

### prepare_line_item



```php
private prepare_line_item(\BigCommerce\Api\v3\Model\BaseItem|\BigCommerce\Api\v3\Model\ItemGiftCertificate $item): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$item` | **\BigCommerce\Api\v3\Model\BaseItem&#124;\BigCommerce\Api\v3\Model\ItemGiftCertificate** |  |





***

### get_product



```php
private get_product(\BigCommerce\Api\v3\Model\BaseItem $item): \BigCommerce\Post_Types\Product\Product
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$item` | **\BigCommerce\Api\v3\Model\BaseItem** |  |





***

### get_terms



```php
private get_terms(mixed $post_id, mixed $taxonomy): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **mixed** |  |
| `$taxonomy` | **mixed** |  |





***

### format_term



```php
private format_term(\WP_term $term): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term` | **\WP_term** |  |





***

### get_variant_sku



```php
private get_variant_sku(int $variant_id, \BigCommerce\Post_Types\Product\Product $product): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$variant_id` | **int** |  |
| `$product` | **\BigCommerce\Post_Types\Product\Product** |  |





***

### get_options



```php
private get_options(\BigCommerce\Api\v3\Model\BaseItem $item): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$item` | **\BigCommerce\Api\v3\Model\BaseItem** |  |





***

### get_variant



```php
private get_variant(int $variant_id, \BigCommerce\Post_Types\Product\Product $product): object|null
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$variant_id` | **int** |  |
| `$product` | **\BigCommerce\Post_Types\Product\Product** |  |





***

### get_max_quantity



```php
private get_max_quantity(mixed $order_max, mixed $inventory): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$order_max` | **mixed** |  |
| `$inventory` | **mixed** |  |





***

### format_currency



```php
private format_currency(mixed $value): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** |  |





***

### prepare_base_item



```php
private prepare_base_item(\BigCommerce\Api\v3\Model\BaseItem $item): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$item` | **\BigCommerce\Api\v3\Model\BaseItem** |  |





***

### prepare_gift_certificate_item



```php
private prepare_gift_certificate_item(\BigCommerce\Api\v3\Model\ItemGiftCertificate $item): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$item` | **\BigCommerce\Api\v3\Model\ItemGiftCertificate** |  |





***

### calculate_total_tax



```php
private calculate_total_tax(float $cart_amount, float $discount_amount, float $coupons_discount_amount, array $items): float
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart_amount` | **float** | The `cart_amount` value for the cart |
| `$discount_amount` | **float** | The `discount_amount` value for the cart |
| `$coupons_discount_amount` | **float** | The `coupons_discount_amount` value for the cart |
| `$items` | **array** | The items in the cart |





***

### identify_channel

Identify the channel associated with the cart

```php
private identify_channel(): void
```












***

### get_thumbnail_id



```php
private get_thumbnail_id(\BigCommerce\Post_Types\Product\Product $product, mixed $variant_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Post_Types\Product\Product** |  |
| `$variant_id` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
