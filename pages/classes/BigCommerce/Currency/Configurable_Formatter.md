***

# Configurable_Formatter

Class for configuring and formatting currency values.

Allows for customizable currency symbol, position, and decimal precision when formatting monetary values.

* Full name: `\BigCommerce\Currency\Configurable_Formatter`
* This class implements:
[`\BigCommerce\Currency\Currency_Formatter`](./Currency_Formatter.md)




## Methods


### __construct

Constructor for Configurable_Formatter.

```php
public __construct(string $symbol = &#039;¤&#039;, string $symbol_position = Position::POSITION_LEFT, int $decimals = 2): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$symbol` | **string** | The currency symbol to use (default is &#039;¤&#039;). |
| `$symbol_position` | **string** | The position of the currency symbol, using constants from `Position` (default is left). |
| `$decimals` | **int** | The number of decimal places for formatted values (default is 2). |





***

### format

Formats a currency value based on the configured settings.

```php
public format(float $value): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **float** | The numeric value to format. |


**Return Value:**

The formatted currency value with the symbol in the configured position.




***


***
> Automatically generated on 2024-12-10
