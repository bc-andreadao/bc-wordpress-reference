***

# Formatter_Factory

Factory class to create and manage currency formatters.



* Full name: `\BigCommerce\Currency\Formatter_Factory`



## Properties


### formatters

Cache of created currency formatters.

```php
private array $formatters
```






***

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

### auto_format



```php
private auto_format(): mixed
```












***

### enabled_currencies



```php
private enabled_currencies(): mixed
```












***

### make_auto_formatter



```php
private make_auto_formatter(mixed $currency_code): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$currency_code` | **mixed** |  |





***

### make_configurable_formatter_from_currency



```php
private make_configurable_formatter_from_currency(mixed $currency): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$currency` | **mixed** |  |





***

### make_configurable_formatter_from_options



```php
private make_configurable_formatter_from_options(): mixed
```












***


***
> Automatically generated on 2024-12-10
