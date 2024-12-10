***

# Cart





* Full name: `\BigCommerce\Settings\Sections\Cart`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;cart&#039;|
|`OPTION_ENABLE_CART`|public| |&#039;bigcommerce_enable_cart&#039;|
|`OPTION_AJAX_CART`|public| |&#039;bigcommerce_ajax_cart&#039;|
|`OPTION_CART_PAGE_ID`|public| |\BigCommerce\Pages\Cart_Page::NAME|
|`OPTION_EMBEDDED_CHECKOUT`|public| |&#039;bigcommerce_enable_embedded_checkout&#039;|


## Methods


### __construct



```php
public __construct(\BigCommerce\Pages\Cart_Page $cart_page, \BigCommerce\Pages\Checkout_Page $checkout_page, \BigCommerce\Pages\Checkout_Complete_Page $checkout_complete_page): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart_page` | **\BigCommerce\Pages\Cart_Page** |  |
| `$checkout_page` | **\BigCommerce\Pages\Checkout_Page** |  |
| `$checkout_complete_page` | **\BigCommerce\Pages\Checkout_Complete_Page** |  |





***

### register_settings_section



```php
public register_settings_section(): void
```












***

### render_section



```php
public render_section(mixed $section): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$section` | **mixed** |  |





***

### render_checkout_docs_url



```php
public render_checkout_docs_url(): mixed
```












***

### render_enable_cart_field



```php
public render_enable_cart_field(): mixed
```












***

### render_ajax_cart_field



```php
public render_ajax_cart_field(): mixed
```












***

### render_embedded_checkout_field



```php
public render_embedded_checkout_field(): mixed
```












***

### render_cart_page_field



```php
public render_cart_page_field(): mixed
```












***


## Inherited methods


### render_field



```php
public render_field(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### render_number_field



```php
public render_number_field(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### get_disabled_attr_headless

Get disabled attribute if headless option is on

```php
public get_disabled_attr_headless(): string
```












***

### render_page_field



```php
public render_page_field(mixed $args): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
