***

# Headless_Product_Processor





* Full name: `\BigCommerce\Import\Processors\Headless_Product_Processor`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`HEADLESS_CURSOR`|public| |&#039;bigcommerce_gql_next_cursor&#039;|
|`HEADLESS_PRODUCTS`|public| |&#039;bigcommerce_gql_products_process&#039;|
|`HEADLESS_CHANNEL`|public| |&#039;bigcommerce_gql_active_channel&#039;|

## Properties


### status



```php
private \BigCommerce\Import\Runner\Status $status
```






***

### requester



```php
private \BigCommerce\GraphQL\GraphQL_Processor $requester
```






***

### channel_term



```php
private \WP_Term $channel_term
```






***

### batch



```php
private int|mixed $batch
```






***

### api



```php
private \BigCommerce\Api\v3\Api\CatalogApi $api
```






***

## Methods


### __construct



```php
public __construct(\BigCommerce\Api\v3\Api\CatalogApi $api, \BigCommerce\Import\Runner\Status $status, \BigCommerce\GraphQL\GraphQL_Processor $requester, mixed $channel_term, mixed $batch = 50): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\v3\Api\CatalogApi** |  |
| `$status` | **\BigCommerce\Import\Runner\Status** |  |
| `$requester` | **\BigCommerce\GraphQL\GraphQL_Processor** |  |
| `$channel_term` | **mixed** |  |
| `$batch` | **mixed** |  |





***

### run

Fetch products data via GraphQL and process it

```php
public run(): void
```












***

### process_data



```php
protected process_data(mixed $data): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **mixed** |  |





***

### get_bc_slugs



```php
protected get_bc_slugs(mixed $product_ids): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_ids` | **mixed** |  |





***

### update_product_slug



```php
protected update_product_slug(mixed $post_id, mixed $slug): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **mixed** |  |
| `$slug` | **mixed** |  |





***

### process_single_edge



```php
protected process_single_edge(mixed $edge, mixed $product_id, mixed $title): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$edge` | **mixed** |  |
| `$product_id` | **mixed** |  |
| `$title` | **mixed** |  |





***

### save_terms



```php
protected save_terms(mixed $edge, mixed $post_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$edge` | **mixed** |  |
| `$post_id` | **mixed** |  |





***

### build_terms



```php
private build_terms(mixed $categories, mixed $brand_id): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$categories` | **mixed** |  |
| `$brand_id` | **mixed** |  |





***

### map_product_categories



```php
private map_product_categories(array $bc_category_ids): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_category_ids` | **array** |  |





***

### map_brand



```php
private map_brand(array $bc_brand_ids): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_brand_ids` | **array** |  |





***

### is_product_exist

Check if product is already imported

```php
protected is_product_exist(mixed $product_id): false|int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **mixed** |  |





***

### get_option_name



```php
private get_option_name(): mixed
```












***


***
> Automatically generated on 2024-12-10