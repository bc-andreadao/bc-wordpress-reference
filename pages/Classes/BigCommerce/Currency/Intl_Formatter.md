***

# Intl_Formatter

Formatter class for currency values using PHP's intl extension.



* Full name: `\BigCommerce\Currency\Intl_Formatter`
* This class implements:
[`\BigCommerce\Currency\Currency_Formatter`](./classes/BigCommerce/Currency/Currency_Formatter.md)




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
> Automatically generated on 2025-01-07
