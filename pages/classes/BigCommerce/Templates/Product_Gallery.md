***

# Product_Gallery





* Full name: `\BigCommerce\Templates\Product_Gallery`
* Parent class: [`\BigCommerce\Templates\Controller`](./classes/BigCommerce/Templates/Controller.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`PRODUCT`|public| |&#039;product&#039;|
|`IMAGE_IDS`|public| |&#039;image_ids&#039;|
|`YOUTUBE_VIDEOS`|public| |&#039;youtube_videos&#039;|
|`FALLBACK`|public| |&#039;fallback_image&#039;|
|`SIZE`|public| |&#039;image_size&#039;|
|`THUMBNAIL`|public| |&#039;thumbnail_size&#039;|
|`ZOOM`|public| |&#039;zoom&#039;|
|`ZOOM_SIZE`|public| |&#039;zoom_size&#039;|
|`CDN_IMAGES`|public| |&#039;cdn_images&#039;|

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

### zoom_size



```php
protected zoom_size(): mixed
```












***

### get_data

Build the data that will be available to the template

```php
public get_data(): array
```












***

### get_fallback



```php
protected get_fallback(): mixed
```












***

### get_videos



```php
protected get_videos(\BigCommerce\Post_Types\Product\Product $product): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Post_Types\Product\Product** |  |





***

### get_wrapper_classes

Add a class with the image size we're using

```php
protected get_wrapper_classes(): string[]
```












***

### enable_zoom



```php
protected enable_zoom(): mixed
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

### get_images_cdn_url

Get list of cdn url for each image

```php
public get_images_cdn_url(array $images_ids = []): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$images_ids` | **array** |  |





***

### get_headless_images



```php
public get_headless_images(\BigCommerce\Post_Types\Product\Product $product): array|array[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Post_Types\Product\Product** |  |





***


***
> Automatically generated on 2024-12-13
