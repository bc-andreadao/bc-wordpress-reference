***

# Gutenberg_Block

A base class for creating Gutenberg blocks in BigCommerce.



* Full name: `\BigCommerce\Editor\Gutenberg\Blocks\Gutenberg_Block`
* This class is an **Abstract class**


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public|string|&#039;&#039;|


## Methods


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
> Automatically generated on 2025-01-14
