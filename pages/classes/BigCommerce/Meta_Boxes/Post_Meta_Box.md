***

# Post_Meta_Box





* Full name: `\BigCommerce\Meta_Boxes\Post_Meta_Box`
* Parent class: [`\BigCommerce\Meta_Boxes\Meta_Box`](./classes/BigCommerce/Meta_Boxes/Meta_Box.md)
* This class is an **Abstract class**




## Methods


### register



```php
public register(string $post_type = &#039;&#039;, \WP_Post $post = null): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_type` | **string** |  |
| `$post` | **\WP_Post** |  |





***

### save_post



```php
public save_post(int $post_id, \WP_Post $post): void
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** |  |
| `$post` | **\WP_Post** |  |





***

### get_post_types



```php
protected get_post_types(): string[]
```




* This method is **abstract**.




**Return Value:**

The post types to which this metabox applies




***


## Inherited methods


### register



```php
public register(): void
```












***

### get_name



```php
protected get_name(): string
```




* This method is **abstract**.




**Return Value:**

The unique identifier for the metabox




***

### get_title



```php
protected get_title(): string
```




* This method is **abstract**.




**Return Value:**

The title of the metabox




***

### render

Render the metabox contents

```php
public render(object $object): void
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$object` | **object** |  |





***

### get_screen



```php
protected get_screen(): string|array|null
```









**Return Value:**

The screens on which to display the metabox




***

### get_context



```php
protected get_context(): string
```









**Return Value:**

One of 'normal', 'side', or 'advanced'




***

### get_priority



```php
protected get_priority(): string
```









**Return Value:**

One of 'high', 'core', 'default', 'low'




***

### get_callback_args



```php
protected get_callback_args(): null|array
```









**Return Value:**

Additional args to pass to the render callback




***


***
> Automatically generated on 2025-01-07
