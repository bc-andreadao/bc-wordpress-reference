***

# Product_Form_Preview

A specialized version of the product form that disables purchase functionality.

It hides product options and renders a disabled purchase button.

* Full name: `\BigCommerce\Templates\Product_Form_Preview`
* Parent class: [`\BigCommerce\Templates\Product_Form`](./Product_Form.md)



## Properties


### template

The template path for rendering the product form preview.

```php
protected string $template
```






***

## Methods


### parse_options

Parses the options for the product form preview.

```php
protected parse_options(array $options): array
```

Ensures that options are never displayed.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$options` | **array** | The original options array. |


**Return Value:**

The modified options array with options hidden.




***

### get_data

Retrieves data for rendering the product form preview.

```php
public get_data(): array
```

Temporarily adds a filter to overwrite the purchase button HTML.







**Return Value:**

The data array for rendering the product form preview.




***

### overwrite_purchase_button

Overwrites the purchase button with a disabled button in the product form preview.

```php
public overwrite_purchase_button(string $html, int $post_id, string $label): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$html` | **string** | The original button HTML. |
| `$post_id` | **int** | The product post ID. |
| `$label` | **string** | The label for the button. |


**Return Value:**

The modified button HTML with a disabled state.




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

### get_options



```php
protected get_options(\BigCommerce\Post_Types\Product\Product $product): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Post_Types\Product\Product** |  |


**Return Value:**

The rendered option and modifier fields for the product




***


***
> Automatically generated on 2024-12-10
