***

# Cart





* Full name: `\BigCommerce\Templates\Cart`
* Parent class: [`\BigCommerce\Templates\Controller`](./Controller.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CART`|public| |&#039;cart&#039;|
|`ERROR_MESSAGE`|public| |&#039;error_message&#039;|
|`COUPON_CODE`|public| |&#039;coupon_code&#039;|
|`HEADER`|public| |&#039;header&#039;|
|`ITEMS`|public| |&#039;items&#039;|
|`FOOTER`|public| |&#039;footer&#039;|

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

### get_error_message



```php
protected get_error_message(): mixed
```












***

### get_header



```php
protected get_header(): mixed
```












***

### get_coupon_code



```php
protected get_coupon_code(mixed $cart): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart` | **mixed** |  |





***

### get_items



```php
protected get_items(mixed $cart): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart` | **mixed** |  |





***

### get_footer



```php
protected get_footer(mixed $cart): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart` | **mixed** |  |





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