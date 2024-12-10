***

# Template_Override

Class Template_Override

Tell WordPress about the path to the templates

* Full name: `\BigCommerce\Templates\Template_Override`




## Methods


### render_product_single

Render the contents of the product single template

```php
public render_product_single(int $post_id): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** |  |





***

### render_product_archive

Render the contents of the product archive template

```php
public render_product_archive(): string
```












***

### set_product_single_template_path



```php
public set_product_single_template_path(string[] $templates): string[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$templates` | **string[]** |  |





***

### set_product_archive_template_path



```php
public set_product_archive_template_path(string[] $templates): string[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$templates` | **string[]** |  |





***

### set_search_template_path



```php
public set_search_template_path(string[] $templates): string[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$templates` | **string[]** |  |





***

### set_taxonomy_archive_template_path



```php
public set_taxonomy_archive_template_path(string[] $templates): string[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$templates` | **string[]** |  |





***

### prefix_theme_paths

Prefix all paths with the theme's plugin override dir

```php
private prefix_theme_paths(string[] $paths): string[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$paths` | **string[]** |  |





***

### include_product_template



```php
public include_product_template(string|bool $template): string|bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template` | **string&#124;bool** |  |





***

### get_product_single_path



```php
private get_product_single_path(): bool|string
```









**Return Value:**

Path to the product single template in the plugin




***

### get_product_archive_path



```php
private get_product_archive_path(): bool|string
```









**Return Value:**

Path to the product archive template in the plugin




***

### get_template_path

Get the template path

```php
private get_template_path(string $relative_path): string|bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$relative_path` | **string** |  |





***


***
> Automatically generated on 2024-12-10
