***

# Products





* Full name: `\BigCommerce\Shortcodes\Products`
* This class implements:
[`\BigCommerce\Shortcodes\Shortcode`](./Shortcode.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bigcommerce_product&#039;|

## Properties


### shortcode_rest_controller



```php
private \BigCommerce\Rest\Shortcode_Controller $shortcode_rest_controller
```






***

## Methods


### default_attributes



```php
public static default_attributes(): mixed
```



* This method is **static**.








***

### __construct



```php
public __construct(mixed $shortcode_controller): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$shortcode_controller` | **mixed** |  |





***

### render

Return the rendered markup for this shortcode.

```php
public render(mixed $attr, mixed $instance): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attr` | **mixed** |  |
| `$instance` | **mixed** |  |





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


***
> Automatically generated on 2024-12-10
