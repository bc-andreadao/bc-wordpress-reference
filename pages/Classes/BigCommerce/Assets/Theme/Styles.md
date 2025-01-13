***

# Styles

Manages the enqueuing of CSS stylesheets for the theme. This includes handling the inclusion of
asset files and applying any filters to the stylesheet before it is enqueued. It also checks the
theme settings to conditionally load the styles based on user preferences.



* Full name: `\BigCommerce\Assets\Theme\Styles`




## Methods


### __construct

Styles constructor.

```php
public __construct(string $asset_directory, string $version): mixed
```

Initializes the Styles class with the asset directory and version.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$asset_directory` | **string** | The path to the plugin assets directory. |
| `$version` | **string** | The version of the asset build. |





***

### enqueue_styles

Enqueues the CSS styles for the frontend.

```php
public enqueue_styles(): mixed
```

This method registers and enqueues the main stylesheet, allowing for customization of the
stylesheet filename through filters. It also conditionally loads the stylesheet based on
the theme settings (e.g., whether the full CSS file should be loaded).










***


***
> Automatically generated on 2025-01-13
