***

# Null_Theme

A placeholder class for themes that do not require any compatibility layer.

This class extends the base Theme class but does not add any additional functionality.

* Full name: `\BigCommerce\Compatibility\Themes\Null_Theme`
* Parent class: [`\BigCommerce\Compatibility\Themes\Theme`](./classes/BigCommerce/Compatibility/Themes/Theme.md)






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
> Automatically generated on 2025-01-03
