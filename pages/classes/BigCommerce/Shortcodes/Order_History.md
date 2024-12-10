***

# Order_History

Provides a shortcode to display the order history for logged-in users.

Handles rendering both the order history list and individual order details.

* Full name: `\BigCommerce\Shortcodes\Order_History`
* This class implements:
[`\BigCommerce\Shortcodes\Shortcode`](./Shortcode.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public|string|&#039;bigcommerce_order_history&#039;|
|`ORDER_ID_QUERY_ARG`|public|string|&#039;order_id&#039;|

## Properties


### rest_controller



```php
private \BigCommerce\Rest\Orders_Shortcode_Controller $rest_controller
```






***

## Methods


### __construct

Constructor for the Order_History class.

```php
public __construct(\BigCommerce\Rest\Orders_Shortcode_Controller $rest_controller): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$rest_controller` | **\BigCommerce\Rest\Orders_Shortcode_Controller** | The REST controller used for AJAX requests. |





***

### default_attributes

Get the default attributes for the order history shortcode.

```php
public static default_attributes(): array
```



* This method is **static**.





**Return Value:**

Default attributes including pagination, per-page limits, and AJAX settings.




***

### render

Render the order history or order details based on the attributes and query parameters.

```php
public render(array $attr, mixed $instance): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attr` | **array** | Shortcode attributes. |
| `$instance` | **mixed** | The current instance (not used). |


**Return Value:**

The rendered HTML output or an empty string for unauthorized users.




***

### render_history_list



```php
private render_history_list(mixed $attr): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attr` | **mixed** |  |





***

### render_order_details



```php
private render_order_details(mixed $attr, mixed $order_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attr` | **mixed** |  |
| `$order_id` | **mixed** |  |





***

### get_orders



```php
private get_orders(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***

### get_total_pages



```php
private get_total_pages(mixed $per_page): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$per_page` | **mixed** |  |





***

### next_page_url



```php
private next_page_url(array $attr, mixed $max_pages): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attr` | **array** |  |
| `$max_pages` | **mixed** |  |





***

### per_page_default



```php
private per_page_default(): mixed
```












***


***
> Automatically generated on 2024-12-10
