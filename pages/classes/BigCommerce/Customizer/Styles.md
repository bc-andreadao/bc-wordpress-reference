***

# Styles

This class handles the customization of CSS styles for BigCommerce components.

It loads and manipulates a CSS template file and outputs dynamic styles based on theme settings.

* Full name: `\BigCommerce\Customizer\Styles`



## Properties


### template_file

Path to the CSS template file.

```php
private string $template_file
```






***

### black

The color black from the Colors class.

```php
private string $black
```






***

### white

The color white.

```php
private string $white
```






***

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

### using_plugin_css



```php
private using_plugin_css(): bool
```












***

### button_color



```php
private button_color(): mixed
```












***

### button_text



```php
private button_text(): mixed
```












***

### sale_color



```php
private sale_color(): mixed
```












***

### sale_text



```php
private sale_text(): mixed
```












***

### availability_color



```php
private availability_color(): mixed
```












***

### condition_color



```php
private condition_color(): mixed
```












***

### condition_text



```php
private condition_text(): mixed
```












***


***
> Automatically generated on 2024-12-10
