***

# Intl_Formatter

Formatter class for currency values using PHP's intl extension.



* Full name: `\BigCommerce\Currency\Intl_Formatter`
* This class implements:
[`\BigCommerce\Currency\Currency_Formatter`](./Currency_Formatter.md)



## Properties


### formatter

The NumberFormatter instance for formatting currency values.

```php
private \NumberFormatter $formatter
```






***

### currency

The currency code used for formatting.

```php
private string $currency
```






***

## Methods


### __construct

Initializes the Intl_Formatter with a specific currency code.

```php
public __construct(string $currency): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$currency` | **string** | The currency code (e.g., USD, EUR). |





***

### get_locale



```php
private get_locale(): mixed
```












***

### format

Formats a numeric value as a currency string.

```php
public format(float|int|string $value): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **float&#124;int&#124;string** | The value to format. |


**Return Value:**

The formatted currency value.




***


***
> Automatically generated on 2024-12-10
