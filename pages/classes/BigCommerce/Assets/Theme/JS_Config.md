***

# JS_Config

Handles the configuration for JavaScript data, which includes store settings,
product messages, channel data, and other theme-specific data required for the frontend.



* Full name: `\BigCommerce\Assets\Theme\JS_Config`



## Properties


### data



```php
private array $data
```






***

### directory



```php
private string $directory
```






***

### connections



```php
private \BigCommerce\Taxonomies\Channel\Connections $connections
```






***

## Methods


### __construct

JS_Config constructor.

```php
public __construct(string $asset_directory, \BigCommerce\Taxonomies\Channel\Connections $connections): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$asset_directory` | **string** | The directory path where theme assets are stored. |
| `$connections` | **\BigCommerce\Taxonomies\Channel\Connections** | The Connections object used to get channel-related data. |





***

### get_data

Retrieves the configuration data for JavaScript.

```php
public get_data(): array
```

This method fetches the data used in JavaScript files, including store domain, product messages,
channel data, currency information, and the logout URL. If the data has already been generated,
it returns the cached version.







**Return Value:**

The configuration data for JavaScript.




***

### get_current_channel_data



```php
private get_current_channel_data(): mixed
```












***


***
> Automatically generated on 2024-12-10