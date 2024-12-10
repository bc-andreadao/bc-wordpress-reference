***

# Scripts

Manages the enqueuing of JavaScript files for the theme. It handles the inclusion of asset files,
conditional script loading based on page type, and localization of JavaScript data.



* Full name: `\BigCommerce\Assets\Theme\Scripts`



## Properties


### directory



```php
private string $directory
```






***

### version



```php
private string $version
```






***

### config



```php
private \BigCommerce\Assets\Theme\JS_Config $config
```






***

### localization



```php
private \BigCommerce\Assets\Theme\JS_Localization $localization
```






***

## Methods


### __construct

Scripts constructor.

```php
public __construct(string $asset_directory, string $version, \BigCommerce\Assets\Theme\JS_Config $config, \BigCommerce\Assets\Theme\JS_Localization $localization): mixed
```

Initializes the Scripts class with the asset directory, version, and necessary dependencies.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$asset_directory` | **string** | The path to the plugin assets directory. |
| `$version` | **string** | The version of the asset build. |
| `$config` | **\BigCommerce\Assets\Theme\JS_Config** | The JS_Config object for configuration data. |
| `$localization` | **\BigCommerce\Assets\Theme\JS_Localization** | The JS_Localization object for localized strings. |





***

### enqueue_scripts

Enqueues JavaScript files for the frontend.

```php
public enqueue_scripts(): mixed
```

This method registers and enqueues the necessary JavaScript files for the theme, including
manifest, vendor, and plugin scripts. It also conditionally loads the BigCommerce checkout SDK
if the current page is the checkout page.










***


***
> Automatically generated on 2024-12-10
