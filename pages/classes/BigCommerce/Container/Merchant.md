***

# Merchant

Handles merchant-related onboarding and account management for BigCommerce integration.

Provides functionality for creating and connecting merchant accounts, checking account
statuses, and setting up the onboarding API.

* Full name: `\BigCommerce\Container\Merchant`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`MIDDLEMAN_URL`|public|string|&#039;merchant.middleman.url&#039;|
|`ONBOARDING_API`|public|string|&#039;merchant.onboarding.api&#039;|
|`CREATE_ACCOUNT`|public|string|&#039;merchant.onboarding.create_account&#039;|
|`CONNECT_ACCOUNT`|public|string|&#039;merchant.onboarding.connect_account&#039;|
|`ACCOUNT_STATUS`|public|string|&#039;merchant.onboarding.account_status&#039;|
|`SETUP_STATUS`|public|string|&#039;merchant.onboarding.setup_status&#039;|


## Methods


### register

Registers services into the dependency container.

```php
public register(\Pimple\Container $container): void
```

Sets up account onboarding services including account creation, connection,
status checks, and setup status.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container. |





***


***
> Automatically generated on 2024-12-13
