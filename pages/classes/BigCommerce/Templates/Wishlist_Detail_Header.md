***

# Wishlist_Detail_Header





* Full name: `\BigCommerce\Templates\Wishlist_Detail_Header`
* Parent class: [`\BigCommerce\Templates\Controller`](./Controller.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`WISHLIST`|public| |&#039;wishlist&#039;|
|`TITLE`|public| |&#039;title&#039;|
|`SHARE`|public| |&#039;share&#039;|
|`EDIT`|public| |&#039;edit&#039;|
|`DELETE`|public| |&#039;delete&#039;|
|`ACTIONS`|public| |&#039;actions&#039;|

## Properties


### template



```php
protected $template
```






***

## Methods


### parse_options



```php
protected parse_options(array $options): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$options` | **array** |  |





***

### get_data

Build the data that will be available to the template

```php
public get_data(): array
```












***

### render_share_form



```php
private render_share_form(\BigCommerce\Accounts\Wishlists\Wishlist $wishlist): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wishlist` | **\BigCommerce\Accounts\Wishlists\Wishlist** |  |





***

### render_edit_form



```php
private render_edit_form(\BigCommerce\Accounts\Wishlists\Wishlist $wishlist): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wishlist` | **\BigCommerce\Accounts\Wishlists\Wishlist** |  |





***

### render_delete_form



```php
private render_delete_form(\BigCommerce\Accounts\Wishlists\Wishlist $wishlist): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wishlist` | **\BigCommerce\Accounts\Wishlists\Wishlist** |  |





***

### render_actions



```php
private render_actions(\BigCommerce\Accounts\Wishlists\Wishlist $wishlist): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wishlist` | **\BigCommerce\Accounts\Wishlists\Wishlist** |  |





***

### get_edit_wishlist_action



```php
private get_edit_wishlist_action(\BigCommerce\Accounts\Wishlists\Wishlist $wishlist): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wishlist` | **\BigCommerce\Accounts\Wishlists\Wishlist** |  |





***

### get_delete_wishlist_action



```php
private get_delete_wishlist_action(\BigCommerce\Accounts\Wishlists\Wishlist $wishlist): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wishlist` | **\BigCommerce\Accounts\Wishlists\Wishlist** |  |





***


## Inherited methods


### format_currency

Formats a numeric value as a currency string.

```php
protected format_currency(float $value, string $empty_value = &#039;&#039;): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **float** | The currency value to format. |
| `$empty_value` | **string** | The value to return if $value is empty. Pass `null` to format anyway. |


**Return Value:**

The formatted currency string or the empty value.




***

### factory

Creates an instance of the controller

```php
public static factory(array $options = [], string $template = &#039;&#039;): static
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$options` | **array** |  |
| `$template` | **string** |  |





***

### __construct



```php
public __construct(array $options = [], string $template = &#039;&#039;): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$options` | **array** |  |
| `$template` | **string** |  |





***

### parse_options



```php
protected parse_options(array $options): array
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$options` | **array** |  |





***

### render

Render the template and return it as a string

```php
public render(): string
```









**Return Value:**

The rendered template




***

### get_data

Build the data that will be available to the template

```php
public get_data(): array
```




* This method is **abstract**.







***

### get_template



```php
private get_template(string $relative_path): \BigCommerce\Templates\Template
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$relative_path` | **string** |  |





***

### wrap

Wrap the template output in an optional tag. This provides us a mechanism
to ensure that some elements and classes are consistently available
for JavaScript targeting, despite possible template overrides.

```php
protected wrap(string $html): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$html` | **string** |  |





***

### get_wrapper_tag



```php
protected get_wrapper_tag(): mixed
```












***

### get_wrapper_classes



```php
protected get_wrapper_classes(): mixed
```












***

### get_wrapper_attributes



```php
protected get_wrapper_attributes(): mixed
```












***

### build_attribute_string

Build a string of HTML attributes that can safely be
injected into a template out of a list of key/value pairs

```php
protected build_attribute_string(array $attributes): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attributes` | **array** |  |





***


***
> Automatically generated on 2024-12-10