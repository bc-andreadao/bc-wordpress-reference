***

# Scripts

Handles the enqueueing and registration of admin scripts and Gutenberg-specific scripts.



* Full name: `\BigCommerce\Assets\Admin\Scripts`




## Methods


### __construct

Constructor.

```php
public __construct(string $asset_directory, string $version, \BigCommerce\Assets\Admin\JS_Config $config, \BigCommerce\Assets\Admin\JS_Localization $localization): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$asset_directory` | **string** | Path to the plugin assets directory. |
| `$version` | **string** | Asset build version. |
| `$config` | **\BigCommerce\Assets\Admin\JS_Config** | Configuration object for JavaScript. |
| `$localization` | **\BigCommerce\Assets\Admin\JS_Localization** | Localization object for JavaScript. |





***

### enqueue_scripts

Enqueue admin and Gutenberg scripts.

```php
public enqueue_scripts(): mixed
```

Registers and enqueues required scripts, and localizes them with configuration
and localization data. Delays certain script outputs until after the admin footer scripts.










***

### print_footer_scripts

Print footer scripts.

```php
public print_footer_scripts(): mixed
```

Enqueues the admin scripts and reprocesses the script queue
to ensure correct execution timing.










***


***
> Automatically generated on 2025-01-03
