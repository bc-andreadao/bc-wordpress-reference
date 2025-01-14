***

# Product_Archive

Customizer settings and controls for the Product Archive section.

This class defines constants and methods to register and manage customizer
options for the product catalog, including settings for sorting, filtering,
slugs, and layout.

* Full name: `\BigCommerce\Customizer\Sections\Product_Archive`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public|string|&#039;bigcommerce_product_archive&#039;|
|`ARCHIVE_TITLE`|public|string|&#039;bigcommerce_product_archive_title&#039;|
|`ARCHIVE_SLUG`|public|string|&#039;bigcommerce_product_archive_slug&#039;|
|`ARCHIVE_DESCRIPTION`|public|string|&#039;bigcommerce_product_archive_description&#039;|
|`SORT_OPTIONS`|public|string|&#039;bigcommerce_product_archive_sort_options&#039;|
|`FILTER_OPTIONS`|public|string|&#039;bigcommerce_product_archive_filter_options&#039;|
|`CATEGORY_SLUG`|public|string|&#039;bigcommerce_category_archive_slug&#039;|
|`BRAND_SLUG`|public|string|&#039;bigcommerce_brand_archive_slug&#039;|
|`SORT_FEATURED`|public|string|&#039;featured&#039;|
|`SORT_DATE`|public|string|&#039;date&#039;|
|`SORT_SALES`|public|string|&#039;sales&#039;|
|`SORT_TITLE_ASC`|public|string|&#039;title_asc&#039;|
|`SORT_TITLE_DESC`|public|string|&#039;title_desc&#039;|
|`SORT_REVIEWS`|public|string|&#039;reviews&#039;|
|`SORT_PRICE_ASC`|public|string|&#039;price_asc&#039;|
|`SORT_PRICE_DESC`|public|string|&#039;price_desc&#039;|
|`SORT_INVENTORY_COUNT`|public|string|&#039;inventory_count&#039;|
|`SORT_SKU`|public|string|&#039;sku&#039;|
|`FILTER_CATEGORY`|public|string|\BigCommerce\Taxonomies\Product_Category\Product_Category::NAME|
|`FILTER_BRAND`|public|string|\BigCommerce\Taxonomies\Brand\Brand::NAME|
|`PER_PAGE_DEFAULT`|public|int|24|
|`PER_PAGE`|public|string|&#039;bigcommerce_products_per_page&#039;|
|`GRID_COLUMNS`|public|string|&#039;bigcommerce_catalog_grid_columns&#039;|
|`QUICK_VIEW`|public|string|&#039;bigcommerce_enable_quick_view&#039;|
|`SEARCH_FIELD`|public|string|&#039;bigcommerce_catalog_enable_search_field&#039;|
|`GENERAL_INVENTORY`|public|string|&#039;bigcommerce_general_inventory_settings&#039;|


## Methods


### register

Registers customizer settings and controls for the product archive section.

```php
public register(\WP_Customize_Manager $wp_customize): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_customize` | **\WP_Customize_Manager** | WordPress Customizer manager instance. |





***

### sort_choices

Retrieves the available sorting choices for the product catalog.

```php
public static sort_choices(): array
```



* This method is **static**.





**Return Value:**

An associative array of sorting choices with keys and labels.




***

### sanitize_sort

Sanitizes and validates the sorting choices.

```php
public sanitize_sort(array|string $values): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$values` | **array&#124;string** | The sorting choices input to sanitize. |


**Return Value:**

Sanitized sorting choices.




***

### filter_choices

Retrieves filtering choices for the BigCommerce catalog.

```php
public static filter_choices(): array
```



* This method is **static**.





**Return Value:**

The filtering options available.




***

### sanitize_filter

Sanitizes the provided filter values to ensure they match available choices.

```php
public sanitize_filter(array|string $values): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$values` | **array&#124;string** | The filter values to sanitize. |


**Return Value:**

The sanitized filter values.




***

### get_field_description

Gets the field description for display in the WordPress Customizer.

```php
public get_field_description(): string
```









**Return Value:**

The description HTML or an empty string.




***


***
> Automatically generated on 2025-01-14
