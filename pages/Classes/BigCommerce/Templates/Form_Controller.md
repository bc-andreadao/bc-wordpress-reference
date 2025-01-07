***

# Form_Controller





* Full name: `\BigCommerce\Templates\Form_Controller`
* Parent class: [`\BigCommerce\Templates\Controller`](./classes/BigCommerce/Templates/Controller.md)
* This class is an **Abstract class**


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`DEFAULTS`|public| |&#039;defaults&#039;|
|`ERRORS`|public| |&#039;errors&#039;|

## Properties


### submission_key



```php
protected $submission_key
```







***

## Methods


### get_data

Build the data that will be available to the template

```php
public get_data(): array
```












***

### get_form_defaults



```php
protected get_form_defaults(): mixed
```












***

### restore_submission

If the user has submitted the form, restore their submission
so they don't have to re-type everything

```php
protected restore_submission(string $field, array $data, array $submission): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$field` | **string** | The name of the field containing the values to restore |
| `$data` | **array** | The default data to render in the form |
| `$submission` | **array** | The data the user submitted |





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
