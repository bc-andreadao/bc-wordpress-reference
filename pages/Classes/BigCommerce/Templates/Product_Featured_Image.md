***

# Product_Featured_Image





* Full name: `\BigCommerce\Templates\Product_Featured_Image`
* Parent class: [`\BigCommerce\Templates\Controller`](./classes/BigCommerce/Templates/Controller.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`PRODUCT`|public| |&#039;product&#039;|
|`ATTACHMENT_ID`|public| |&#039;attachment_id&#039;|
|`IMAGE`|public| |&#039;image&#039;|
|`SIZE`|public| |&#039;size&#039;|
|`CLASSES`|public| |&#039;classes&#039;|

## Properties


### template



```php
protected $template
```







***

### wrapper_tag



```php
protected string $wrapper_tag
```







***

### wrapper_classes



```php
protected string[] $wrapper_classes
```







***

### cdn_image



```php
protected $cdn_image
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

### get_attachment_id



```php
protected get_attachment_id(\BigCommerce\Post_Types\Product\Product $product): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Post_Types\Product\Product** |  |





***

### get_image



```php
protected get_image(mixed $attachment_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attachment_id` | **mixed** |  |





***

### get_wrapper_classes



```php
protected get_wrapper_classes(): mixed
```












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
> Automatically generated on 2025-01-07