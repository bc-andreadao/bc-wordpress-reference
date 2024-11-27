***

# Checkout

Registers checkout-related functionality for the BigCommerce platform, including customer login and checkout requirements.

This class extends the Provider class and interacts with various BigCommerce services, such as customer login and checkout
requirements, through a Pimple container.

* Full name: `\BigCommerce\Container\Checkout`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`REQUIREMENTS_NOTICE`|public|string|&#039;checkout.requirements_notice&#039;|
|`LOGIN`|public|string|&#039;checkout.customer_login&#039;|


## Methods


### register

Registers the checkout-related functionality in the container.

```php
public register(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The Pimple container to register services in. |





***

### requirements



```php
private requirements(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### customer_login



```php
private customer_login(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***


***
> Automatically generated on 2024-11-27
