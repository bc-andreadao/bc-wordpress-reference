***

# Formatter_Factory

Factory class to create and manage currency formatters.



* Full name: `\BigCommerce\Currency\Formatter_Factory`




## Methods


### get

Retrieves a currency formatter for the given currency code.

```php
public get(string $currency_code): \BigCommerce\Currency\Intl_Formatter|\BigCommerce\Currency\Configurable_Formatter
```

Creates a new formatter if one does not already exist for the currency code.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$currency_code` | **string** | The currency code for which to retrieve the formatter. |


**Return Value:**

The currency formatter.




***


***
> Automatically generated on 2025-01-03
