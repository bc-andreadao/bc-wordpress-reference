***

# Post_Types

Handles the management of custom post types, particularly for products in the WordPress admin interface.

This class integrates with various hooks and filters to customize post behavior, including slug management, permalink modification,
featured image handling, and custom product status for unsupported products.

It also interfaces with the BigCommerce API to manage import processes, prevent publication of certain posts, and manage product deletion.

* Full name: `\BigCommerce\Container\Post_Types`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`PRODUCT`|public|string|&#039;post_type.product&#039;|
|`PRODUCT_CONFIG`|public|string|&#039;post_type.product.config&#039;|
|`PRODUCT_QUERY`|public|string|&#039;post_type.product.query&#039;|
|`PRODUCT_ADMIN`|public|string|&#039;post_type.product.admin&#039;|
|`PRODUCT_UNSUPPORTED`|public|string|&#039;post_type.product.unsupported&#039;|
|`PRODUCT_DELETION`|public|string|&#039;post_type.product.deletion&#039;|
|`STORE_LINKS`|public|string|&#039;post_type.product.store_links&#039;|
|`CHANNEL_INDICATOR`|public|string|&#039;post_type.product.channel_indicator&#039;|
|`CHANNEL_SYNC`|public|string|&#039;post_type.product.channel_sync&#039;|
|`PRODUCT_ADMIN_LIST`|public|string|&#039;post_type.product.admin_list&#039;|
|`PRODUCT_UNIQUE_SLUG`|public|string|&#039;post_type.product.unique_slug&#039;|
|`LISTING_RESET`|public|string|&#039;post_type.product.listing_reset&#039;|
|`PRODUCT_RESYNC`|public|string|&#039;post_type.product.resync_single&#039;|
|`PRODUCT_SEO`|public|string|&#039;post_type.product.seo&#039;|
|`CART_INDICATOR`|public|string|&#039;post_type.page.cart_indicator&#039;|
|`CART_CREATOR`|public|string|&#039;post_type.page.cart_creator&#039;|
|`QUEUE`|public|string|&#039;post_type.queue_task&#039;|
|`QUEUE_CONFIG`|public|string|&#039;post_type.queue_task.config&#039;|
|`SYNC_LOG`|public|string|&#039;post_type.sync_log&#039;|
|`SYNC_LOG_CONFIG`|public|string|&#039;post_type.sync_log.config&#039;|
|`WPGRAPHQL_PRODUCTS`|public|string|&#039;bigcommerce.wpgrapql_products&#039;|
|`WPGRAPHQL_CONFIG`|public|string|&#039;bigcommerce.wpgrapql_config&#039;|


## Methods


### register

Registers all post types and hooks them into the container.

```php
public register(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The Pimple container. |





***

### product

Configures product-related dependencies in the container.

```php
private product(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The Pimple container. |





***

### queue

Queues the configuration for the Queue_Task.

```php
private queue(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The service container. |





***

### sync_log

Sets up the synchronization logging.

```php
private sync_log(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The service container. |





***

### product_store_links

Adds product store links to various admin actions.

```php
private product_store_links(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The service container. |





***

### product_listing_reset

Resets product listings based on specific actions.

```php
private product_listing_reset(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The service container. |





***

### product_resync

Resyncs a single product based on user action.

```php
private product_resync(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The service container. |





***

### product_channel_indicator

Adds a channel indicator for products when enabled.

```php
private product_channel_indicator(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The service container. |





***

### channel_sync

Synchronizes product data with external channels.

```php
private channel_sync(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The service container. |





***

### product_slugs

Adds unique slugs for products based on the channel context.

```php
private product_slugs(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The service container. |





***

### product_seo

Handles product SEO settings.

```php
private product_seo(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The service container. |





***


***
> Automatically generated on 2024-12-10