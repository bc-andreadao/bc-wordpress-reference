***

# Amp_Template_Override

Class Amp_Template_Override

Responsible for overriding template paths to provide AMP-specific
versions when AMP mode is enabled.

* Full name: `\BigCommerce\Amp\Amp_Template_Override`




## Methods


### __construct

Constructor for the Amp_Template_Override class.

```php
public __construct(string $amp_directory = &#039;amp&#039;): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$amp_directory` | **string** | Name of the directory containing AMP template overrides. Default is &#039;amp&#039;. |





***

### override_template_path

Filters the path to a requested template, providing AMP-specific versions if available.

```php
public override_template_path(string $path, string $relative_path): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$path` | **string** | The absolute path to the requested template. |
| `$relative_path` | **string** | The relative path of the template within the theme/plugin. |


**Return Value:**

The filtered template path, modified for AMP if applicable.




***

### override_classic_amp_template_path

Overrides template paths for classic AMP templates.

```php
public override_classic_amp_template_path(string $file, string $template_type, \WP_Post $post): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$file` | **string** | The absolute path to the AMP template. |
| `$template_type` | **string** | The type of template being served (e.g., single, archive). |
| `$post` | **\WP_Post** | The current post object. |


**Return Value:**

The overridden template path.




***

### override_classic_header_bar_template

Overrides the header bar template for AMP classic mode.

```php
public override_classic_header_bar_template(string $file, string $type, array $container): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$file` | **string** | Template file path. |
| `$type` | **string** | Template type (e.g., &#039;header-bar&#039;). |
| `$container` | **array** | \BigCommerce\Container\Amp |


**Return Value:**

The overridden template file path.




***

### is_classic

Determines whether AMP is in classic mode.

```php
public is_classic(): bool
```

Classic mode renders AMP templates for all pages, while paired/native mode only
renders AMP templates for specific components.







**Return Value:**

True if classic mode is enabled; false otherwise.




***

### provide_header_nav_menu

Provides the header navigation menu data in AMP classic mode.

```php
public provide_header_nav_menu(array $data): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **array** | AMP template data. |


**Return Value:**

Filtered data with `header_nav_menu` included.




***


***
> Automatically generated on 2025-01-13
