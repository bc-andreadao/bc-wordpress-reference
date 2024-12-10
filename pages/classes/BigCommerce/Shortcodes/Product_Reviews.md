***

# Product_Reviews





* Full name: `\BigCommerce\Shortcodes\Product_Reviews`
* This class implements:
[`\BigCommerce\Shortcodes\Shortcode`](./Shortcode.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bigcommerce_reviews&#039;|


## Methods


### default_attributes

Set default attributes

```php
public static default_attributes(): array
```



* This method is **static**.








***

### render

Return the rendered markup for this shortcode.

```php
public render(array $attributes, int $instance): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attributes` | **array** | key id is expected |
| `$instance` | **int** |  |





***

### next_page_url

Build the URL for the next page of reviews

```php
private next_page_url(int $post_id, int $per_page, int $current_page, int $max_pages): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** |  |
| `$per_page` | **int** |  |
| `$current_page` | **int** |  |
| `$max_pages` | **int** |  |





***


***
> Automatically generated on 2024-12-10
