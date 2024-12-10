***

# JS_Config

Handles the configuration for JavaScript assets in the BigCommerce admin.

This includes paths to images and icons, as well as various settings related
to product categories, flags, brands, and AJAX actions used in the admin interface.

* Full name: `\BigCommerce\Assets\Admin\JS_Config`



## Properties


### data



```php
private $data
```






***

### gutenberg



```php
private $gutenberg
```






***

### directory



```php
private $directory
```






***

## Methods


### __construct

Constructor

```php
public __construct(string $asset_directory): mixed
```

Initializes the JS_Config object with a specified asset directory.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$asset_directory` | **string** | The directory containing the assets. |





***

### get_data

Get JS configuration data

```php
public get_data(): array
```

Retrieves the JavaScript configuration data, including paths for images and icons,
as well as other relevant settings such as product categories and AJAX actions.







**Return Value:**

The JavaScript configuration data.




***

### get_gutenberg_data

Get Gutenberg JS configuration data

```php
public get_gutenberg_data(): array
```

Retrieves the Gutenberg-specific JavaScript configuration data.







**Return Value:**

The Gutenberg JavaScript configuration data.




***


***
> Automatically generated on 2024-12-10
