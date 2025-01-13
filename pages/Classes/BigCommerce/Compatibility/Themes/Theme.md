***

# Theme

Base class for themes, providing functionality for rendering templates and checking version compatibility.

Specific theme implementations should extend this class and define templates and their supported versions.

* Full name: `\BigCommerce\Compatibility\Themes\Theme`
* This class is an **Abstract class**



## Properties


### supported_version



```php
protected $supported_version
```







***

### templates



```php
protected $templates
```







***

## Methods


### render_template

Render the specified theme template with options.

```php
public render_template(string $template_name, array $options = []): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template_name` | **string** | The name of the template to render. |
| `$options` | **array** | The options to pass to the template controller. |





***

### load_compat_functions

Load theme-specific compatibility functions.

```php
public load_compat_functions(): void
```

This method is intended to be overridden by child classes to load additional functions.










***

### is_version_supported

Check if the theme version is supported.

```php
public is_version_supported(string $version): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$version` | **string** | The version to check. |


**Return Value:**

True if the version is supported, false otherwise.




***


***
> Automatically generated on 2025-01-13
