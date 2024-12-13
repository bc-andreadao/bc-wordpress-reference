***

# Order_Details





* Full name: `\BigCommerce\Templates\Order_Details`
* Parent class: [`\BigCommerce\Templates\Order_Summary`](./classes/BigCommerce/Templates/Order_Summary.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ORDER`|public| |&#039;order&#039;|
|`PRODUCTS`|public| |&#039;products&#039;|
|`SHIPMENTS`|public| |&#039;shipments&#039;|

## Properties


### template



```php
protected $template
```







***

## Methods


### get_data

Build the data that will be available to the template

```php
public get_data(): array
```












***

### get_products



```php
protected get_products(mixed $order): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$order` | **mixed** |  |





***

### get_shipments



```php
protected get_shipments(mixed $order): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$order` | **mixed** |  |





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

### get_payment_method



```php
protected get_payment_method(mixed $method): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$method` | **mixed** |  |





***

### get_support_email



```php
protected get_support_email(): mixed
```












***

### get_fallback_image



```php
protected get_fallback_image(mixed $size): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$size` | **mixed** |  |





***

### identify_channel



```php
protected identify_channel(mixed $order): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$order` | **mixed** |  |





***


***
> Automatically generated on 2024-12-13
