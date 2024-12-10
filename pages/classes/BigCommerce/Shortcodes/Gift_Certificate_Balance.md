***

# Gift_Certificate_Balance





* Full name: `\BigCommerce\Shortcodes\Gift_Certificate_Balance`
* This class implements:
[`\BigCommerce\Shortcodes\Shortcode`](./Shortcode.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bigcommerce_gift_balance&#039;|

## Properties


### api



```php
private \BigCommerce\Api\Marketing_Api $api
```






***

## Methods


### __construct



```php
public __construct(\BigCommerce\Api\Marketing_Api $api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\Marketing_Api** |  |





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

### get_balance



```php
private get_balance(mixed $code): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$code` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
