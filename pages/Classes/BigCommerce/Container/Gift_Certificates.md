***

# Gift_Certificates

This class provides functionality for registering and handling the gift certificates sub-navigation
in the BigCommerce environment. It extends the Provider class and implements a registration method
to add a sub-navigation to the content.



* Full name: `\BigCommerce\Container\Gift_Certificates`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`SUB_NAV`|public|string|&#039;gift_certificates.sub_nav&#039;|


## Methods


### register

Registers the gift certificates sub-navigation service and hooks the sub-navigation to the content.

```php
public register(\Pimple\Container $container): mixed
```

This method registers the `SUB_NAV` service in the container and defines a callback that inserts
the gift certificates sub-navigation above the content. The callback is hooked into the `the_content`
filter to ensure the sub-navigation is added to the content when it is being rendered.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The Pimple container instance used for managing dependencies. |





***


***
> Automatically generated on 2025-01-14
