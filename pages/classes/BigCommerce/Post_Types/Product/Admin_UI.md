***

# Admin_UI





* Full name: `\BigCommerce\Post_Types\Product\Admin_UI`




## Methods


### prevent_slug_changes

Prevent updates to the post slug

```php
public prevent_slug_changes(array $post_data, array $submitted_data): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_data` | **array** |  |
| `$submitted_data` | **array** |  |





***

### override_sample_permalink_html

Filters the sample permalink HTML markup to make it a static link

```php
public override_sample_permalink_html(string $html, int $post_id, string $title, string $slug, \WP_Post $post): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$html` | **string** | Sample permalink HTML markup. |
| `$post_id` | **int** | Post ID. |
| `$title` | **string** | New sample permalink title. |
| `$slug` | **string** | New sample permalink slug. |
| `$post` | **\WP_Post** | Post object. |





***

### remove_featured_image_meta_box

Remove the featured image metabox to prevent
editing of the automatically assigned featured image

```php
public remove_featured_image_meta_box(\WP_Post $post): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post` | **\WP_Post** |  |





***

### list_table_import_status

Add the last import date at the end of the views above the products
list table. While not exactly a view, it's a reasonable place
to inject the status into the UI.

```php
public list_table_import_status(array $views = []): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$views` | **array** |  |





***

### list_import_tooltip

Adds an import tooltip to products page

```php
public list_import_tooltip(array $views = []): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$views` | **array** |  |





***

### list_table_manage_link

Add a link to manage products in BigCommerce to the top
of the products list table

```php
public list_table_manage_link(array $views = []): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$views` | **array** |  |





***

### last_import_date



```php
public last_import_date(): string
```









**Return Value:**

The date of the last import. Empty if not available.




***

### list_table_admin_notices

Show applicable admin notices at the top of the products list table

```php
public list_table_admin_notices(): void
```












***


***
> Automatically generated on 2025-01-07
