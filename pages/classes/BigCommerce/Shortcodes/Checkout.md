***

# Checkout





* Full name: `\BigCommerce\Shortcodes\Checkout`
* This class implements:
[`\BigCommerce\Shortcodes\Shortcode`](./Shortcode.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bigcommerce_checkout&#039;|

## Properties


### cart_api



```php
private \BigCommerce\Api\v3\Api\CartApi $cart_api
```






***

## Methods


### __construct



```php
public __construct(\BigCommerce\Api\v3\Api\CartApi $cart_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart_api` | **\BigCommerce\Api\v3\Api\CartApi** |  |





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


***
> Automatically generated on 2024-12-10