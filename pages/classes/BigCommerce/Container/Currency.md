***

# Currency

Currency container provider class.

This class provides the necessary bindings for currency functionality, including
currency code, currency formatter, and related services. It handles the registration
of currency-related services and hooks for filtering currency values in BigCommerce.

* Full name: `\BigCommerce\Container\Currency`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CURRENCY`|public|string|&#039;currency&#039;|
|`FORMATTER`|public|string|&#039;currency.formatter&#039;|
|`FACTORY`|public|string|&#039;currency.formatter.factory&#039;|
|`CURRENCY_CODE`|public|string|&#039;currency.code&#039;|


## Methods


### register

Registers the services and hooks related to currency functionality.

```php
public register(\Pimple\Container $container): mixed
```

This method binds the currency manager, formatter, and formatter factory to the
container. It also sets up various filters for modifying currency values and currency
codes based on the configured currency for the store.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The container instance to register services with. |





***


***
> Automatically generated on 2024-12-31
