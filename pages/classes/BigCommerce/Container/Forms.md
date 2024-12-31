***

# Forms

Forms class handles various form actions within BigCommerce, such as registration, address updates, product reviews, and more.

It registers form handlers and provides functionality to process form actions, handle errors, success messages, redirects, and messaging.
This class is part of the container and utilizes dependency injection to manage the various handlers for each action.

* Full name: `\BigCommerce\Container\Forms`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`DELETE_ADDRESS`|public|string|&#039;forms.delete_address&#039;|
|`REGISTER`|public|string|&#039;forms.register&#039;|
|`REVIEW`|public|string|&#039;forms.review&#039;|
|`UPDATE_ADDRESS`|public|string|&#039;forms.update_address&#039;|
|`UPDATE_PROFILE`|public|string|&#039;forms.update_profile&#039;|
|`GIFT_CERTIFICATE`|public|string|&#039;forms.purchase_gift_certificate&#039;|
|`ERRORS`|public|string|&#039;forms.errors&#039;|
|`SUCCESS`|public|string|&#039;forms.success&#039;|
|`REDIRECTS`|public|string|&#039;forms.redirects&#039;|
|`MESSAGING`|public|string|&#039;forms.messaging&#039;|
|`SWITCH_CURRENCY`|public|string|&#039;forms.switch_currency&#039;|


## Methods


### register

Registers all the form actions and handlers into the container.

```php
public register(\Pimple\Container $container): mixed
```

This method sets up actions for handling form submissions, errors, success, redirects, and messaging.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container. |





***


***
> Automatically generated on 2024-12-31
