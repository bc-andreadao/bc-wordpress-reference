***

# Editor_Dialog_Template

A class that handles rendering the editor dialog template with product filtering options.



* Full name: `\BigCommerce\Editor\Editor_Dialog_Template`




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


***
> Automatically generated on 2024-12-10
