***

# Product_Creator

Handles the creation and saving of BigCommerce products into WordPress.



* Full name: `\BigCommerce\Import\Importers\Products\Product_Creator`
* Parent class: [`\BigCommerce\Import\Importers\Products\Product_Saver`](./classes/BigCommerce/Import/Importers/Products/Product_Saver.md)




## Methods


### do_import

Executes the import process for a product.

```php
public do_import(): mixed
```









**Return Value:**

The result of the parent import process.




***

### get_post_array

Retrieves the array of post data to be saved in the WordPress database.

```php
protected get_post_array(\BigCommerce\Import\Importers\Products\Product_Builder $builder): array
```

Adds a default comment status if it is not already set.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$builder` | **\BigCommerce\Import\Importers\Products\Product_Builder** | The product builder instance containing the product data. |


**Return Value:**

The post data array.




***

### send_notifications

Sends notifications after a product has been created via the import process.

```php
protected send_notifications(): void
```

Triggers a custom action hook for other processes to react to the product creation event.










***


## Inherited methods


### __construct

Product_Saver constructor.

```php
public __construct(\BigCommerce\Api\v3\Model\Product $product, \BigCommerce\Api\v3\Model\Listing $listing, \WP_Term $channel_term, \BigCommerce\Api\v3\Api\CatalogApi $catalog, int $post_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Api\v3\Model\Product** | Product data from the BigCommerce API. |
| `$listing` | **\BigCommerce\Api\v3\Model\Listing** | Listing data from the BigCommerce Channel API. |
| `$channel_term` | **\WP_Term** | The WordPress term representing the channel. |
| `$catalog` | **\BigCommerce\Api\v3\Api\CatalogApi** | Instance of the BigCommerce Catalog API. |
| `$post_id` | **int** | The WordPress post ID for the imported product. |





***

### do_import

Imports the product into WordPress by saving the product data, terms, post meta,
and images. Also sends notifications once the import is complete.

```php
public do_import(): int
```









**Return Value:**

The post ID of the imported product.




***

### save_wp_post

Saves the WordPress post data for the imported product.

```php
protected save_wp_post(\BigCommerce\Import\Importers\Products\Product_Builder $builder): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$builder` | **\BigCommerce\Import\Importers\Products\Product_Builder** | The product builder instance used to create post data. |





***

### get_post_array

Builds and retrieves the post data array for the product.

```php
protected get_post_array(\BigCommerce\Import\Importers\Products\Product_Builder $builder): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$builder` | **\BigCommerce\Import\Importers\Products\Product_Builder** | The product builder instance used to create post data. |


**Return Value:**

The post array to be saved in WordPress.




***

### save_wp_postmeta

Saves the product post meta data.

```php
protected save_wp_postmeta(\BigCommerce\Import\Importers\Products\Product_Builder $builder): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$builder` | **\BigCommerce\Import\Importers\Products\Product_Builder** | The product builder instance used to create post meta. |





***

### save_modifiers

Saves product modifier information to the WordPress post.

```php
protected save_modifiers(\BigCommerce\Post_Types\Product\Product $product): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Post_Types\Product\Product** | The product instance. |





***

### save_options

Saves product option information to the WordPress post.

```php
protected save_options(\BigCommerce\Post_Types\Product\Product $product): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Post_Types\Product\Product** | The product instance. |





***

### save_custom_fields

Saves custom fields for the product to the WordPress post.

```php
protected save_custom_fields(\BigCommerce\Post_Types\Product\Product $product): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Post_Types\Product\Product** | The product instance. |





***

### save_terms

Saves taxonomy terms associated with the product to WordPress.

```php
protected save_terms(\BigCommerce\Import\Importers\Products\Product_Builder $builder): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$builder` | **\BigCommerce\Import\Importers\Products\Product_Builder** | The product builder instance used to create terms. |





***

### save_images

Saves feature image and gallery images for the product.

```php
protected save_images(\BigCommerce\Import\Importers\Products\Product_Builder $builder): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$builder` | **\BigCommerce\Import\Importers\Products\Product_Builder** | The product builder instance used to create images. |





***

### send_notifications

Sends notifications after the product import has been completed.

```php
protected send_notifications(): void
```












***


***
> Automatically generated on 2025-01-14
