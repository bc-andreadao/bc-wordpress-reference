***

# Styles

Handles the enqueueing and registration of admin and Gutenberg-specific CSS styles.



* Full name: `\BigCommerce\Assets\Admin\Styles`




## Methods


### __construct

Constructor.

```php
public __construct(string $asset_directory, string $version): mixed
```

Initializes the class with the provided directory path and version.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$asset_directory` | **string** | Path to the plugin assets directory. |
| `$version` | **string** | Asset build version. |





***

### enqueue_styles

Enqueue admin and Gutenberg styles.

```php
public enqueue_styles(): mixed
```

Registers and enqueues the required CSS styles for the BigCommerce admin panel
and Gutenberg editor. The styles are minified for production, with debug support
for unminified versions.










***


***
> Automatically generated on 2025-01-03
