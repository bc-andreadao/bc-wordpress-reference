***

# Banners

This class is responsible for managing the banners service within the dependency injection container.

It provides functionality to register the banners API factory and integrates banner-specific configurations
into JavaScript settings via a filter hook.

The `banners` service is registered, allowing the application to interact with the banners API and manage banner-related data.

* Full name: `\BigCommerce\Container\Banners`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`BANNERS`|public| |&#039;banners&#039;|


## Methods


### register

Registers the banners service and related configuration within the container.

```php
public register(\Pimple\Container $container): void
```

The `banners` service is instantiated with the banners API factory,
allowing the application to manage banners. A filter is also added
to integrate banner-specific configurations into JavaScript settings.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container used to manage services. |





***


***
> Automatically generated on 2025-01-13
