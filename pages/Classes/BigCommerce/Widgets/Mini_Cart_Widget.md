***

# Mini_Cart_Widget

Class Product_Category_Widget

A widget to display a list or dropdown of product categories

* Full name: `\BigCommerce\Widgets\Mini_Cart_Widget`
* Parent class: [`WP_Widget`](./classes/WP_Widget.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bigcommerce_mini_cart&#039;|


## Methods


### __construct

Sets up a new Product Categories widget instance.

```php
public __construct(): mixed
```












***

### widget

Outputs the content for the current Mini Cart widget instance.

```php
public widget(array $args, array $instance): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | Display arguments including &#039;before_title&#039;, &#039;after_title&#039;,<br />&#039;before_widget&#039;, and &#039;after_widget&#039;. |
| `$instance` | **array** | Settings for the current widget instance. |





***

### update

Handles updating settings for the current Product Categories widget instance.

```php
public update(array $new_instance, array $old_instance): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$new_instance` | **array** | New settings for this instance as input by the user via<br />WP_Widget::form(). |
| `$old_instance` | **array** | Old settings for this instance. |


**Return Value:**

Updated settings to save.




***

### form

Outputs the settings form for the Product Categories widget.

```php
public form(array $instance): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$instance` | **array** | Current settings. |





***


***
> Automatically generated on 2025-01-14
