***

# Styles

This class handles the customization of CSS styles for BigCommerce components.

It loads and manipulates a CSS template file and outputs dynamic styles based on theme settings.

* Full name: `\BigCommerce\Customizer\Styles`




## Methods


### __construct

Styles constructor.

```php
public __construct(string $template_file): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template_file` | **string** | Path to the CSS template file. |





***

### get_styles

Retrieves the styles by replacing CSS variables with values from the theme customization.

```php
public get_styles(): string
```









**Return Value:**

The generated CSS styles.




***

### print_styles

Prints the generated styles within a `<style>` tag in the head.

```php
public print_styles(): void
```












***

### print_css

Prints the generated styles directly (without `<style>` tags) in the head.

```php
public print_css(): void
```












***


***
> Automatically generated on 2025-01-14
