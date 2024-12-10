***

# Editor

Loads behavior relevant to the admin post editor, including rendering custom buttons,
templates, and Gutenberg blocks within the WordPress admin interface. It also handles
the integration of the Gutenberg editor with BigCommerce blocks and assets.



* Full name: `\BigCommerce\Container\Editor`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`SHORTCODE_BUTTON`|public|string|&#039;admin.shortcode_button&#039;|
|`UI_DIALOG`|public|string|&#039;admin.ui_dialog&#039;|
|`GUTENBERG_BLOCKS`|public|string|&#039;gutenberg.blocks&#039;|
|`GUTENBERG_MIGRATE`|public|string|&#039;gutenberg.migrate&#039;|
|`STYLES`|public|string|&#039;gutenberg.styles&#039;|


## Methods


### register

Registers the necessary components for the editor, including buttons, dialog templates,
and Gutenberg blocks.

```php
public register(\Pimple\Container $container): mixed
```

This function initializes and sets up the custom behavior for the WordPress admin post
editor, integrating custom buttons and templates for a more enhanced editing experience.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container. |





***


***
> Automatically generated on 2024-12-10
