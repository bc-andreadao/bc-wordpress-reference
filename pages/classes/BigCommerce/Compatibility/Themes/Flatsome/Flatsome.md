***

# Flatsome

This class defines the compatibility layer for the Flatsome theme in the BigCommerce ecosystem.

It specifies the supported version of the theme, maps template files to corresponding template classes,
and loads additional compatibility functions.

* Full name: `\BigCommerce\Compatibility\Themes\Flatsome\Flatsome`
* Parent class: [`\BigCommerce\Compatibility\Themes\Theme`](./classes/BigCommerce/Compatibility/Themes/Theme.md)



## Properties


### supported_version

The supported version of the Flatsome theme.

```php
protected string $supported_version
```







***

### templates

Template files mapped to their corresponding template classes.

```php
protected array $templates
```







***

## Methods


### load_compat_functions

Loads the compatibility functions for the Flatsome theme.

```php
public load_compat_functions(): void
```

This method includes the necessary functions for the Flatsome theme compatibility,
which are stored in a separate file for better maintainability.










***


## Inherited methods


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
> Automatically generated on 2025-01-07
