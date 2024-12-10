***

# Editor_Dialog_Template

A class that handles rendering the editor dialog template with product filtering options.



* Full name: `\BigCommerce\Editor\Editor_Dialog_Template`



## Properties


### template_dir



```php
private string $template_dir
```






***

### rendered



```php
private bool $rendered
```






***

## Methods


### __construct

Editor_Dialog_Template constructor.

```php
public __construct(string $template_dir): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template_dir` | **string** | Path to the templates/public directory. |





***

### js_config

Modify the configuration for the editor dialog.

```php
public js_config(array $config, \BigCommerce\Rest\Products_Controller $products_controller, \BigCommerce\Rest\Shortcode_Controller $shortcode_controller): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **array** | Configuration array. |
| `$products_controller` | **\BigCommerce\Rest\Products_Controller** | The products controller instance. |
| `$shortcode_controller` | **\BigCommerce\Rest\Shortcode_Controller** | The shortcode controller instance. |


**Return Value:**

Modified configuration.




***

### render_dialog_once

Renders the editor dialog template only once to avoid duplication.

```php
public render_dialog_once(): string
```

Gutenberg will load it earlier if enabled. We want to ensure it doesn't
get duplicated in the footer.







**Return Value:**

Rendered dialog HTML.




***

### render_dialog

Renders the full dialog content.

```php
public render_dialog(): string
```









**Return Value:**

Rendered dialog HTML.




***

### query_builder



```php
private query_builder(): mixed
```












***

### get_choices

Reorder the terms so sub-categories get nested bellow its parent

```php
private get_choices(mixed $parent_id, mixed $terms_by_parent, mixed $depth): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$parent_id` | **mixed** |  |
| `$terms_by_parent` | **mixed** |  |
| `$depth` | **mixed** |  |





***

### get_channels



```php
private get_channels(): mixed
```












***

### query_settings



```php
private query_settings(): mixed
```












***

### render_template



```php
private render_template(mixed $filename, mixed $vars): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$filename` | **mixed** |  |
| `$vars` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
