***

# Option_Textarea





* Full name: `\BigCommerce\Templates\Option_Types\Option_Textarea`
* Parent class: [`\BigCommerce\Templates\Option_Types\Option_Type`](./classes/BigCommerce/Templates/Option_Types/Option_Type.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`DEFAULT_VALUE`|public| |&#039;default_value&#039;|
|`MINLENGTH`|public| |&#039;minlength&#039;|
|`MAXLENGTH`|public| |&#039;maxlength&#039;|
|`MAXROWS`|public| |&#039;maxrows&#039;|

## Properties


### template



```php
protected $template
```







***

### wrapper_tag



```php
protected $wrapper_tag
```







***

### wrapper_classes



```php
protected $wrapper_classes
```







***

## Methods


### get_data

Build the data that will be available to the template

```php
public get_data(): array
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

### get_id



```php
protected get_id(): mixed
```












***

### get_label



```php
protected get_label(): mixed
```












***

### get_options



```php
protected get_options(): mixed
```












***

### default_option



```php
protected default_option(): mixed
```












***

### sort_options



```php
protected sort_options(mixed $a, mixed $b): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$a` | **mixed** |  |
| `$b` | **mixed** |  |





***


***
> Automatically generated on 2024-12-31
