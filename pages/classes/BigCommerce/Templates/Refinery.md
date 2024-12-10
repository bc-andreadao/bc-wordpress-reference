***

# Refinery





* Full name: `\BigCommerce\Templates\Refinery`
* Parent class: [`\BigCommerce\Templates\Controller`](./Controller.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`QUERY`|public| |&#039;query&#039;|
|`SEARCH`|public| |&#039;search&#039;|
|`SORT`|public| |&#039;sort&#039;|
|`FILTERS`|public| |&#039;filters&#039;|
|`ACTION`|public| |&#039;action&#039;|

## Properties


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

### get_search



```php
private get_search(\WP_Query $query): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |





***

### get_wrapper_classes



```php
protected get_wrapper_classes(): string[]
```












***

### is_search_enabled



```php
private is_search_enabled(): bool
```












***

### get_sort



```php
private get_sort(\WP_Query $query): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |





***

### get_filters



```php
private get_filters(\WP_Query $query): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |





***

### get_choices

Sorts the categories array nesting child under parent with a preceding '-' for each level

```php
private get_choices(mixed $parent_id, mixed $terms_by_parent, mixed $depth): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$parent_id` | **mixed** |  |
| `$terms_by_parent` | **mixed** |  |
| `$depth` | **mixed** |  |





***

### get_action



```php
private get_action(\WP_Query $query): string|void|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |





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
