***

# Store_Links





* Full name: `\BigCommerce\Post_Types\Product\Store_Links`



## Properties


### api_factory



```php
private \BigCommerce\Api_Factory $api_factory
```






***

## Methods


### __construct



```php
public __construct(\BigCommerce\Api_Factory $api_factory): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api_factory` | **\BigCommerce\Api_Factory** |  |





***

### add_row_action



```php
public add_row_action(array $actions, \WP_Post $post): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$actions` | **array** |  |
| `$post` | **\WP_Post** |  |





***

### add_submitbox_link

Add a link to the "Publish" meta box to
open the product in BigCommerce

```php
public add_submitbox_link(\WP_Post $post): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post` | **\WP_Post** |  |





***

### add_link_to_gutenberg_config



```php
public add_link_to_gutenberg_config(array $data): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **array** |  |





***

### modify_edit_product_links_admin_bar



```php
public modify_edit_product_links_admin_bar(\WP_Admin_Bar $wp_admin_bar): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp_admin_bar` | **\WP_Admin_Bar** |  |





***

### get_bigcommerce_post_url

Get the URL to edit a post in the BigCommerce admin

```php
private get_bigcommerce_post_url(\WP_Post $post): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post` | **\WP_Post** |  |





***

### get_store_url

Get the base URL for the BigCommerce store admin

```php
private get_store_url(): string
```












***


***
> Automatically generated on 2024-12-10