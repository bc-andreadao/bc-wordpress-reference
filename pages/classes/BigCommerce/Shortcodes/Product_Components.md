***

# Product_Components





* Full name: `\BigCommerce\Shortcodes\Product_Components`
* This class implements:
[`\BigCommerce\Shortcodes\Shortcode`](./Shortcode.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bc-component&#039;|


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
public render(mixed $attributes, mixed $instance): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attributes` | **mixed** |  |
| `$instance` | **mixed** |  |





***

### product_not_found

If a product cannot be found, display a message
in place of the requested component

```php
private product_not_found(): string
```












***

### image_size



```php
private image_size(): mixed
```












***


***
> Automatically generated on 2024-12-10
