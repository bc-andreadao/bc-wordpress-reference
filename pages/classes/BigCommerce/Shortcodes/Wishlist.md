***

# Wishlist





* Full name: `\BigCommerce\Shortcodes\Wishlist`
* This class implements:
[`\BigCommerce\Shortcodes\Shortcode`](./Shortcode.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bigcommerce_wish_lists&#039;|
|`LIST_PARAM`|public| |&#039;list&#039;|

## Properties


### wishlists



```php
private \BigCommerce\Api\v3\Api\WishlistsApi $wishlists
```






***

## Methods


### __construct



```php
public __construct(\BigCommerce\Api\v3\Api\WishlistsApi $wishlists): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wishlists` | **\BigCommerce\Api\v3\Api\WishlistsApi** |  |





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

### no_customer_template



```php
private no_customer_template(): mixed
```












***

### not_found_template



```php
private not_found_template(): mixed
```












***


***
> Automatically generated on 2024-12-10