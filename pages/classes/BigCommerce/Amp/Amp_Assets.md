***

# Amp_Assets

Class Amp_Assets

Handles loading styles and scripts needed for AMP functionality and layouts.

* Full name: `\BigCommerce\Amp\Amp_Assets`



## Properties


### directory

Path to the plugin assets directory.

```php
private string $directory
```






***

### asset_directory_url

URL of the plugin asset directory.

```php
private string $asset_directory_url
```






***

### customizer_template_file

Path to the customizer template file.

```php
private string $customizer_template_file
```






***

## Methods


### __construct

Constructor for the Amp_Assets class.

```php
public __construct(string $asset_directory, string $asset_directory_url, string $customizer_template_file): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$asset_directory` | **string** | Path to the plugin assets directory. |
| `$asset_directory_url` | **string** | URL to the plugin asset directory. |
| `$customizer_template_file` | **string** | Path to the customizer template file. |





***

### styles

Outputs custom AMP CSS styles directly in the document.

```php
public styles(): mixed
```

Loads the appropriate stylesheet based on the current page (e.g., cart or general)
and performs necessary adjustments like replacing relative paths with absolute URLs.










***

### scripts

Retrieves AMP script handles.

```php
public scripts(): string[]
```

Relevant only in Classic Mode; component scripts are automatically included
in Native/Paired modes. Used in the `amp_post_template_data` filter.







**Return Value:**

List of script handles.




**See Also:**

* \BigCommerce\Amp\amp_register_default_scripts() - 

***

### filter_stylesheet

Filters the main stylesheet when in AMP paired mode.

```php
public filter_stylesheet(string $stylesheet): string
```

Determines the appropriate stylesheet (debug or minified version) based on the
page type (e.g., cart page or general page).






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$stylesheet` | **string** | Stylesheet file name. |


**Return Value:**

Modified stylesheet file name.




***


***
> Automatically generated on 2024-12-10
