***

# Product_Builder

Responsible for constructing product-related data structures
during the import process for BigCommerce products.



* Full name: `\BigCommerce\Import\Importers\Products\Product_Builder`




## Methods


### __construct

Product_Builder constructor.

```php
public __construct(\BigCommerce\Api\v3\Model\Product $product, \BigCommerce\Api\v3\Model\Listing $listing, \WP_Term $channel_term, \BigCommerce\Api\v3\Api\CatalogApi $api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Api\v3\Model\Product** | The product to import. |
| `$listing` | **\BigCommerce\Api\v3\Model\Listing** | The listing for the product. |
| `$channel_term` | **\WP_Term** | The term representing the channel. |
| `$api` | **\BigCommerce\Api\v3\Api\CatalogApi** | The BigCommerce catalog API instance. |





***

### build_post_array

Builds the post array for creating/updating the WordPress post.

```php
public build_post_array(): array
```









**Return Value:**

The post data array.




***

### build_product_array

Builds an array representing the product data.

```php
public build_product_array(): array
```









**Return Value:**

The product data array.




***

### build_variants

Builds variants for the product using sanitized data.

```php
public build_variants(): array
```









**Return Value:**

The array of variant data.




***

### build_taxonomy_terms

Builds taxonomy terms for the product.

```php
public build_taxonomy_terms(): array
```









**Return Value:**

The taxonomy terms associated with the product.




***

### build_images

Builds product images and associates them with a post parent.

```php
public build_images(int $parent_id): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$parent_id` | **int** | The post that will be set as the attachment parent. |


**Return Value:**

The response containing thumbnails, galleries, and variant image mappings.




***

### build_post_meta

Builds and returns an array of metadata for a product post.

```php
public build_post_meta(): array
```

This function generates metadata for a product by extracting and processing
various attributes such as ID, SKU, ratings, inventory, pricing, and more.
The metadata can be used for storing additional information in the database.







**Return Value:**

Associative array containing product metadata with keys:
- `Product::IMPORTER_VERSION_META_KEY` (string): Importer version.
- `Product::BIGCOMMERCE_ID` (int): BigCommerce product ID.
- `Product::SKU` (string): Product SKU.
- `Product::SKU_NORMALIZED` (string): Normalized product SKU.
- `Product::RATING_META_KEY` (float): Average product rating.
- `Product::REVIEW_COUNT_META_KEY` (int): Number of product reviews.
- `Product::RATING_SUM_META_KEY` (int): Sum of product ratings.
- `Product::SALES_META_KEY` (int): Total product sales.
- `Product::PRICE_META_KEY` (float): Product calculated price.
- `Product::INVENTORY_META_KEY` (int): Inventory level.
- `Product::PRICE_RANGE_META_KEY` (array): Price range information.
- `Product::DATA_HASH_META_KEY` (string): Hash of product and listing data.




***

### hash

Generates a hash for a product and listing.

```php
public static hash(\BigCommerce\Api\v3\Model\Product $product, \BigCommerce\Api\v3\Model\Listing $listing): string
```

This function serializes and combines the provided product and listing data,
then computes an MD5 hash. It is used to create a unique identifier
representing the state of the product and listing.

* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Api\v3\Model\Product** | The product model to hash. |
| `$listing` | **\BigCommerce\Api\v3\Model\Listing** | The listing model to hash. |


**Return Value:**

MD5 hash of the combined product and listing data.




***


## Inherited methods


### sanitize_int

Sanitizes an integer value.

```php
protected sanitize_int(mixed $value): int
```

This method converts a scalar value to an integer. If the value is not
scalar (e.g., an array or object), it returns 0.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** | The value to sanitize. |


**Return Value:**

The sanitized integer value.




***

### sanitize_double

Sanitizes a double (floating-point) value.

```php
protected sanitize_double(mixed $value): float
```

This method converts a scalar value to a double. If the value is not
scalar (e.g., an array or object), it returns 0.0.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** | The value to sanitize. |


**Return Value:**

The sanitized double value.




***

### sanitize_string

Sanitizes a string value.

```php
protected sanitize_string(mixed $value): string
```

This method converts a scalar value to a string. If the value is not
scalar (e.g., an array or object), it returns an empty string.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** | The value to sanitize. |


**Return Value:**

The sanitized string value.




***

### sanitize_bool

Sanitizes a boolean value.

```php
protected sanitize_bool(mixed $value): bool
```

This method converts a scalar value to a boolean. If the value is not
scalar (e.g., an array or object), it returns false.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** | The value to sanitize. |


**Return Value:**

The sanitized boolean value.




***

### sanitize_date

Sanitizes a date value.

```php
protected sanitize_date(mixed $value): string
```

This method formats a `DateTime` object to a string in 'Y-m-d H:i:s' format.
If the value is not a `DateTime` object, it returns the current time in
MySQL format.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** | The value to sanitize. |


**Return Value:**

The sanitized date value in 'Y-m-d H:i:s' format.




***


***
> Automatically generated on 2024-12-10
