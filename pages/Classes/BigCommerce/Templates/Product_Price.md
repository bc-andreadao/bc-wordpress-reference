***

# Product_Price





* Full name: `\BigCommerce\Templates\Product_Price`
* Parent class: [`\BigCommerce\Templates\Controller`](./classes/BigCommerce/Templates/Controller.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`PRODUCT`|public| |&#039;product&#039;|
|`SHOW_DEFAULT`|public| |&#039;show_default&#039;|
|`VISIBLE`|public| |&#039;visible&#039;|
|`PRICE_RANGE`|public| |&#039;price_range&#039;|
|`CALCULATED_RANGE`|public| |&#039;calculated_price_range&#039;|
|`RETAIL_PRICE`|public| |&#039;retail_price&#039;|

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

### wrapper_attributes



```php
protected string[] $wrapper_attributes
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

### get_wrapper_attributes



```php
protected get_wrapper_attributes(): mixed
```












***

### visible_class



```php
protected visible_class(bool|null $show_default): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$show_default` | **bool&#124;null** | Whether to show default pricing. Null to use global setting. |





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