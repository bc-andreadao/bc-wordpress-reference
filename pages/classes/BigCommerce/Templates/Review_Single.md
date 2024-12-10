***

# Review_Single





* Full name: `\BigCommerce\Templates\Review_Single`
* Parent class: [`\BigCommerce\Templates\Controller`](./Controller.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`PRODUCT`|public| |&#039;product&#039;|
|`REVIEW_ID`|public| |&#039;review_id&#039;|
|`POST_ID`|public| |&#039;post_id&#039;|
|`BC_ID`|public| |&#039;bc_id&#039;|
|`TITLE`|public| |&#039;title&#039;|
|`CONTENT`|public| |&#039;content&#039;|
|`STATUS`|public| |&#039;status&#039;|
|`RATING`|public| |&#039;rating&#039;|
|`PERCENTAGE`|public| |&#039;percentage&#039;|
|`EMAIL`|public| |&#039;author_email&#039;|
|`NAME`|public| |&#039;author_name&#039;|
|`DATE`|public| |&#039;date_reviewed&#039;|
|`TIMESTAMP`|public| |&#039;timestamp&#039;|

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

### format_content



```php
private format_content(mixed $content): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$content` | **mixed** |  |





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
