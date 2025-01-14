***

# Account_Links

This class is responsible for generating the account links for the user's account page in the Flatsome theme.

It provides links to the order history, addresses, and wish lists (if enabled), and manages the data
passed to the template for rendering.

* Full name: `\BigCommerce\Compatibility\Themes\Flatsome\Templates\Account_Links`
* Parent class: [`\BigCommerce\Templates\Controller`](./classes/BigCommerce/Templates/Controller.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`LINKS`|public| |&#039;links&#039;|

## Properties


### template

The template file used to render the account links.

```php
protected string $template
```







***

## Methods


### parse_options

Merges the provided options with default values.

```php
protected parse_options(array $options): array
```

This method takes an array of options and merges it with the default options
before returning the final options array.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$options` | **array** | The options to merge with defaults. |


**Return Value:**

The merged options.




***

### get_data

Retrieves the data to be passed to the template.

```php
public get_data(): array
```

This method prepares the data array to include the account links and any other necessary options
for the template rendering.







**Return Value:**

The data array, including the account links.




***

### get_links

Generates the links for the user's account page.

```php
protected get_links(): array
```

This method creates an array of links, including order history, addresses, and wish lists (if enabled),
and returns the array of links to be displayed in the template.







**Return Value:**

An array of links with titles and URLs.




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
> Automatically generated on 2025-01-14
