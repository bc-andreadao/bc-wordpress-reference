***

# Order_History

A block to display the current user's order history.



* Full name: `\BigCommerce\Editor\Gutenberg\Blocks\Order_History`
* Parent class: [`\BigCommerce\Editor\Gutenberg\Blocks\Shortcode_Block`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Shortcode_Block.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public|string|&#039;bigcommerce/order-history&#039;|

## Properties


### icon

The block's icon.

```php
protected string $icon
```







***

### shortcode

The shortcode used for this block.

```php
protected string $shortcode
```







***

## Methods


### title

Returns the block's title.

```php
protected title(): string
```









**Return Value:**

The block's title.




***

### html_title

Returns the HTML title for the block.

```php
protected html_title(): string
```









**Return Value:**

The HTML title.




***

### html_image

Returns the URL of the image associated with the block.

```php
protected html_image(): string
```









**Return Value:**

The image URL.




***

### keywords

Returns an array of keywords related to the block.

```php
protected keywords(): array
```









**Return Value:**

The block's keywords.




***


## Inherited methods


### __construct

Constructor for the block, setting the assets URL.

```php
public __construct(string $assets_url): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$assets_url` | **string** | The URL for assets. |





***

### name

Returns the name of the block.

```php
public name(): string
```









**Return Value:**

The name of the block.




***

### register

Registers the block with Gutenberg.

```php
public register(): void
```












***

### registration_args

Returns the arguments for registering the block.

```php
protected registration_args(): array
```









**Return Value:**

The block registration arguments.




***

### render

Renders the block. The default behavior is to convert the block into a shortcode,
which will then be rendered by do_shortcode.

```php
public render(array $attributes): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attributes` | **array** | The block attributes. |


**Return Value:**

The rendered block content.




***

### attributes

Returns the block's attributes.

```php
protected attributes(): array
```









**Return Value:**

The block attributes.




***

### js_config

Returns the JavaScript configuration for the block.

```php
public js_config(): array
```









**Return Value:**

The block's JS configuration.




***

### image_url

Generates the image URL for the given file.

```php
protected image_url(string $file): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$file` | **string** | The image file name. |


**Return Value:**

The complete URL to the image.




***

### title

Returns the title for the block.

```php
protected title(): string
```




* This method is **abstract**.




**Return Value:**

The block's title.




***

### icon

Returns the icon for the block.

```php
protected icon(): string
```









**Return Value:**

The icon for the block.




***

### category

Returns the category for the block.

```php
protected category(): string
```









**Return Value:**

The category for the block.




***

### keywords

Returns an array of keywords for the block.

```php
protected keywords(): array
```









**Return Value:**

The block's keywords.




***

### shortcode

Returns the shortcode associated with the block.

```php
protected shortcode(): string
```









**Return Value:**

The shortcode for the block.




***

### html_title

Returns the HTML title for the block.

```php
protected html_title(): string
```




* This method is **abstract**.




**Return Value:**

The HTML title for the block.




***

### html_image

Returns the HTML image for the block.

```php
protected html_image(): string
```




* This method is **abstract**.




**Return Value:**

The HTML image for the block.




***


***
> Automatically generated on 2025-01-14
