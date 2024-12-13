***

# Nav_Items_Meta_Box

Responsible for handling the BigCommerce menu items
in the nav menu admin



* Full name: `\BigCommerce\Nav_Menu\Nav_Items_Meta_Box`
* Parent class: [`\BigCommerce\Meta_Boxes\Meta_Box`](./classes/BigCommerce/Meta_Boxes/Meta_Box.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bigcommerce_nav_menu&#039;|
|`ACTION`|public| |&#039;bigcommerce_add_menu_items&#039;|
|`CATEGORIES`|public| |&#039;bigcommerce_categories&#039;|
|`BRANDS`|public| |&#039;bigcommerce_brands&#039;|
|`USER_INITIALIZED`|public| |&#039;bigcommerce_nav_settings_initialized&#039;|


## Methods


### get_name



```php
protected get_name(): string
```









**Return Value:**

The unique identifier for the metabox




***

### get_title



```php
protected get_title(): string
```









**Return Value:**

The title of the metabox




***

### render

Renders the meta box, emulating the markup of the WP
core nav meta boxes to take advantage of the nav JS

```php
public render(object $object): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$object` | **object** |  |





***

### set_nav_menu_screen_options



```php
public set_nav_menu_screen_options(): mixed
```












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

### handle_ajax_request

Handle the ajax request to add our custom menu
item type. Hook in just before the standard
WP handler, which would reject our data.

```php
public handle_ajax_request(): void
```












**See Also:**

* \BigCommerce\Nav_Menu\wp_ajax_add_menu_item - 

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
> Automatically generated on 2024-12-13
