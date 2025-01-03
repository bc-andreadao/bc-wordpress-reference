***

# Theme_Factory

Factory class for creating theme instances based on template name and version.

It supports creating instances of themes such as Flatsome and provides a fallback to a Null_Theme
when the template is unsupported or the version is not compatible.

* Full name: `\BigCommerce\Compatibility\Themes\Theme_Factory`



## Properties


### supported

Supported themes

```php
protected array $supported
```







***

## Methods


### make

Creates an instance of the appropriate theme based on the template and version.

```php
public make(string $template, string $version = &#039;1.0.0&#039;): \BigCommerce\Compatibility\Themes\BigCommerce\Compatibility\Themes\Theme
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template` | **string** | The theme template name. |
| `$version` | **string** | The theme version. |


**Return Value:**

The theme instance, or a Null_Theme if unsupported.




***


***
> Automatically generated on 2025-01-03
