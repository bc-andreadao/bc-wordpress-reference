***

# Shortcode_Block

A Gutenberg Block that acts as a wrapper for a shortcode.



* Full name: `\BigCommerce\Editor\Gutenberg\Blocks\Shortcode_Block`
* Parent class: [`\BigCommerce\Editor\Gutenberg\Blocks\Gutenberg_Block`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Gutenberg_Block.md)
* This class is an **Abstract class**



## Properties


### assets_url

URL for the assets.

```php
protected string $assets_url
```







***

### shortcode

The shortcode associated with the block.

```php
protected string $shortcode
```







***

### icon

The icon for the block.

```php
protected string $icon
```







***

### category

The category under which the block is listed.

```php
protected string $category
```







***

## Methods


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

### js_config

Returns the JavaScript configuration for the block.

```php
public js_config(): array
```









**Return Value:**

The block's JS configuration.




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


## Inherited methods


### __construct

Gutenberg_Block constructor.

```php
public __construct(): mixed
```

Ensures that the extending class defines a NAME constant.









**Throws:**
<p>If NAME constant is not set in the extending class.</p>

- [`LogicException`](./classes/LogicException.md)



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

Render the block to a string. This is called from `do_blocks()`,
which runs on the `the_content` filter.

```php
public render(array $attributes): string
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attributes` | **array** | The block attributes. |


**Return Value:**

The HTML output of the block.




**See Also:**

* \BigCommerce\Editor\Gutenberg\Blocks\do_blocks() - * \BigCommerce\Editor\Gutenberg\Blocks\the_content - 

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

Returns the configuration data to pass to the front-end.

```php
public js_config(): array
```




* This method is **abstract**.




**Return Value:**

The configuration data.




***


***
> Automatically generated on 2024-12-13
