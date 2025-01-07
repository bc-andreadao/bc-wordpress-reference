***

# Checkout

Handles the registration of checkout-related services and actions.

This class is responsible for registering the services related to the checkout
process, such as displaying checkout requirements notices and handling customer
login functionality during the checkout flow.

* Full name: `\BigCommerce\Container\Checkout`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`REQUIREMENTS_NOTICE`|public| |&#039;checkout.requirements_notice&#039;|
|`LOGIN`|public| |&#039;checkout.customer_login&#039;|


## Methods


### register

Registers checkout-related services in the container.

```php
public register(\Pimple\Container $container): mixed
```

This method is used to register the checkout services, including the
requirements notice and customer login services, in the container.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The container to register the services in. |





***


***
> Automatically generated on 2025-01-07
