***

# Currencies

This class handles fetching, processing, and storing currency information from BigCommerce.

It uses the v2 and v3 BigCommerce APIs to retrieve available currencies and their assignments
to channels, and stores the relevant data in WordPress options and term meta.

* Full name: `\BigCommerce\Import\Processors\Currencies`
* This class implements:
[`\BigCommerce\Import\Processors\Import_Processor`](./classes/BigCommerce/Import/Processors/Import_Processor.md)




## Methods


### __construct

Currencies constructor.

```php
public __construct(\BigCommerce\Api\Currencies_Api $currencies_api, \BigCommerce\Api\v3\Api\CurrencyApi $currencyV3, \BigCommerce\Taxonomies\Channel\Connections $connections): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$currencies_api` | **\BigCommerce\Api\Currencies_Api** |  |
| `$currencyV3` | **\BigCommerce\Api\v3\Api\CurrencyApi** |  |
| `$connections` | **\BigCommerce\Taxonomies\Channel\Connections** |  |





***

### run

Runs the currency fetching and processing routine.

```php
public run(): void
```

Fetches currencies using the v2 API, filters enabled currencies, stores them in options, and processes channel currencies.










***

### process_channel_currencies

Retrieves currencies set for each channel and stores them in term meta.

```php
public process_channel_currencies(): void
```

This process is only performed for MSF (Multi-Storefront) stores.










***


***
> Automatically generated on 2025-01-07
