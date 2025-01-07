***

# Banners

Handles the management and display of banners on various pages of the BigCommerce WordPress theme. It
provides methods to configure JavaScript settings, fetch banners from the API, and filter banners based
on the current page context, visibility, and date range.



* Full name: `\BigCommerce\Banners\Banners`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CACHE`|public|string|&#039;bigcommerce_banners&#039;|
|`CACHE_TTL`|public|int|&#039;3600&#039;|
|`PAGE_HOME`|public|string|&#039;home_page&#039;|
|`PAGE_CATEGORY`|public|string|&#039;category_page&#039;|
|`PAGE_BRAND`|public|string|&#039;brand_page&#039;|
|`PAGE_SEARCH`|public|string|&#039;search_page&#039;|
|`DATE_TYPE_CUSTOM`|public|string|&#039;custom&#039;|


## Methods


### __construct

Banners constructor.

```php
public __construct(object $banners_api): mixed
```

Initializes the Banners class with a banners API instance.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$banners_api` | **object** | The banners API instance. |





***

### js_config

Adds banner configuration to the JS config.

```php
public js_config(array $config): array
```

This method adds the banner settings, including background color, text color, and the context-based
banners, to the JavaScript configuration. The configuration is later localized in the theme.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **array** | The current JavaScript configuration. |


**Return Value:**

The modified JavaScript configuration.




***

### get_context_banners

Retrieves banners for the current page context.

```php
public get_context_banners(): array
```

This method filters banners based on the current page type (home, category, brand, search), visibility,
and any custom date ranges that are defined for each banner. Only banners that match the current context
will be returned.







**Return Value:**

The filtered list of banners for the current context.




***

### get_banners

Fetches banners from the banners API.

```php
public get_banners(): array
```

This method checks for cached banners and fetches them from the API if they are not already cached.
The fetched banners are stored in the WordPress transient cache for future use.







**Return Value:**

The list of banners retrieved from the API or cache.




***


***
> Automatically generated on 2025-01-07
