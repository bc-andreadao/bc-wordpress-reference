***

# JS_Localization

Class JS_Localization

Provides the localization strings needed for the admin JavaScript files.
These strings include messages, button labels, and error messages that are
used in the admin UI and are available for translation.

* Full name: `\BigCommerce\Assets\Admin\JS_Localization`




## Methods


### get_data

Stores all text strings needed in the admin scripts.js file

```php
public get_data(): array
```

The code below is an example of structure. Check the readme js section for more info on how to use.










***

### kses_strings

Recursively sanitize all the strings with wp_kses

```php
private kses_strings(string[]|string $strings): array|string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$strings` | **string[]&#124;string** | The strings to sanitize. |


**Return Value:**

The sanitized strings.




***


***
> Automatically generated on 2024-12-10
