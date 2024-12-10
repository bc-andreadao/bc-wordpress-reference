***

# Template_Compatibility

Provides compatibility functionality to override WooCommerce page templates.

This class handles the removal of WooCommerce-specific templates from the page template hierarchy.

* Full name: `\BigCommerce\Compatibility\Template_Compatibility`




## Methods


### override_page_template

Overrides the page template for WooCommerce pages that assume WooCommerce functions will be available.

```php
public override_page_template(string $template, string $type, array $templates): string
```

If a theme has a page template (e.g., `page-cart.php`) that relies on WooCommerce functions,
this method will remove that template from the hierarchy to prevent errors if WooCommerce is not present.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template` | **string** | The current template being used for the page. |
| `$type` | **string** | The type of template being overridden. |
| `$templates` | **array** | List of available templates in the hierarchy. |


**Return Value:**

The modified template, or the original template if no changes were made.




***


***
> Automatically generated on 2024-12-10
