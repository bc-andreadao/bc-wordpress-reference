***

# Cache_Control

Class Cache_Control

Handles caching logic based on the presence of specific shortcodes in the content of a singular page.
If certain shortcodes are found, it disables caching for that page.

* Full name: `\BigCommerce\Cart\Cache_Control`




## Methods


### check_for_shortcodes

Checks for specific shortcodes in the content of the queried object.

```php
public check_for_shortcodes(string[] $shortcodes): void
```

If any shortcode is found, it triggers the 'bigcommerce/do_not_cache' action to prevent caching of the page.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$shortcodes` | **string[]** | An array of shortcodes to check for in the post content. |





***

### do_not_cache

Disables caching for the page by sending the appropriate no-cache headers
and defining constants to prevent caching mechanisms from caching the page.

```php
public do_not_cache(): void
```












***


***
> Automatically generated on 2024-12-10
