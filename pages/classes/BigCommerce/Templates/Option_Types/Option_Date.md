***

# Option_Date





* Full name: `\BigCommerce\Templates\Option_Types\Option_Date`
* Parent class: [`\BigCommerce\Templates\Option_Types\Option_Type`](./Option_Type.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`DEFAULT_VALUE`|public| |&#039;default_value&#039;|
|`MIN_VALUE`|public| |&#039;min_value&#039;|
|`MAX_VALUE`|public| |&#039;max_value&#039;|

## Properties


### template



```php
protected $template
```






***

### wrapper_t



```php
protected $wrapper_t
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

### get_default_value



```php
private get_default_value(mixed $config): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **mixed** |  |





***

### get_min_value



```php
private get_min_value(mixed $config): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **mixed** |  |





***

### get_max_value



```php
private get_max_value(mixed $config): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **mixed** |  |





***

### format_date



```php
private format_date(mixed $date_string): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$date_string` | **mixed** |  |





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
> Automatically generated on 2024-12-10