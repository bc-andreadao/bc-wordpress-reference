***

# Currency





* Full name: `\BigCommerce\Settings\Sections\Currency`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;currency&#039;|
|`ENABLED_CURRENCIES`|public| |&#039;bigcommerce_enabled_currencies&#039;|
|`CHANNEL_CURRENCY_CODE`|public| |&#039;bigcommerce_channel_currency_code&#039;|
|`CHANNEL_ALLOWED_CURRENCY`|public| |&#039;bigcommerce_allowed_channel_currencies&#039;|
|`CURRENCY_CODE`|public| |&#039;bigcommerce_currency_code&#039;|
|`CURRENCY_SYMBOL`|public| |&#039;bigcommerce_currency_symbol&#039;|
|`CURRENCY_SYMBOL_POSITION`|public| |&#039;bigcommerce_currency_symbol_position&#039;|
|`INTEGER_UNITS`|public| |&#039;bigcommerce_integer_units&#039;|
|`DECIMAL_UNITS`|public| |&#039;bigcommerce_decimal_units&#039;|
|`PRICE_DISPLAY`|public| |&#039;bigcommerce_price_display&#039;|
|`POSITION_LEFT`|public| |&#039;left&#039;|
|`POSITION_RIGHT`|public| |&#039;right&#039;|
|`POSITION_LEFT_SPACE`|public| |&#039;left+space&#039;|
|`POSITION_RIGHT_SPACE`|public| |&#039;right+space&#039;|
|`DISPLAY_TAX_INCLUSIVE`|public| |&#039;tax_inclusive&#039;|
|`DISPLAY_TAX_EXCLUSIVE`|public| |&#039;tax_exclusive&#039;|
|`ENABLE_CURRENCY_SWITCHER`|public| |&#039;enable_currency_switcher&#039;|


## Methods


### register_settings_section



```php
public register_settings_section(): void
```












***

### render_section



```php
public render_section(mixed $section): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$section` | **mixed** |  |





***

### render_price_display_field



```php
public render_price_display_field(): mixed
```












***

### render_enable_currency_switcher



```php
public render_enable_currency_switcher(): mixed
```












***


## Inherited methods


### render_field



```php
public render_field(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### render_number_field



```php
public render_number_field(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### get_disabled_attr_headless

Get disabled attribute if headless option is on

```php
public get_disabled_attr_headless(): string
```












***


***
> Automatically generated on 2024-12-13
