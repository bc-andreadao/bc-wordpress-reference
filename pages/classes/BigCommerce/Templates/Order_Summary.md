***

# Order_Summary





* Full name: `\BigCommerce\Templates\Order_Summary`
* Parent class: [`\BigCommerce\Templates\Controller`](./Controller.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ORDER`|public| |&#039;order&#039;|
|`THUMBNAIL_SIZE`|public| |&#039;thumbnail_size&#039;|
|`DATE_FORMAT`|public| |&#039;date_format&#039;|
|`ORDER_ID`|public| |&#039;order_id&#039;|
|`DESCRIPTION`|public| |&#039;description&#039;|
|`SHIPPING`|public| |&#039;shipping&#039;|
|`TAX`|public| |&#039;tax&#039;|
|`DISCOUNT`|public| |&#039;discount_amount&#039;|
|`COUPON`|public| |&#039;coupon_amount&#039;|
|`SUBTOTAL`|public| |&#039;subtotal&#039;|
|`TOTAL_EX_TAX`|public| |&#039;total_ex_tax&#039;|
|`TOTAL`|public| |&#039;total&#039;|
|`COUNT`|public| |&#039;item_count&#039;|
|`PAYMENT_METHOD`|public| |&#039;payment_method&#039;|
|`STORE_CREDIT`|public| |&#039;store_credit&#039;|
|`GIFT_CERTIFICATE`|public| |&#039;gift_certificate&#039;|
|`CREATED`|public| |&#039;created_date&#039;|
|`UPDATED`|public| |&#039;updated_date&#039;|
|`SHIPPED`|public| |&#039;shipped_date&#039;|
|`IMAGE_ID`|public| |&#039;image_id&#039;|
|`IMAGE`|public| |&#039;image&#039;|
|`STATUS`|public| |&#039;status&#039;|
|`DETAILS_URL`|public| |&#039;details_url&#039;|
|`SUPPORT_EMAIL`|public| |&#039;support_email&#039;|

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
> Automatically generated on 2024-12-10
