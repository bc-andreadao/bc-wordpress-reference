***

# Widgets

Registers and manages widgets for the application.

Includes widgets for product categories, mini cart, and currency switcher.

* Full name: `\BigCommerce\Container\Widgets`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`WIDGET_LIST`|public|string|&#039;widgets.list&#039;|


## Methods


### register

Registers the widgets and initializes the widget registration action.

```php
public register(\Pimple\Container $container): mixed
```

Registers a list of widgets and hooks them into WordPress using `widgets_init`.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The service container to register services into. |





***


***
> Automatically generated on 2025-01-03
