***

# Customer_Login

Handles customer login logic during the checkout process.



* Full name: `\BigCommerce\Checkout\Customer_Login`




## Methods


### __construct

Constructor for the `Customer_Login` class.

```php
public __construct(\BigCommerce\Merchant\Onboarding_Api $onboarding, \BigCommerce\Api\Store_Api $store): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$onboarding` | **\BigCommerce\Merchant\Onboarding_Api** | API instance for onboarding. |
| `$store` | **\BigCommerce\Api\Store_Api** | API instance for store interactions. |





***

### set_login_token_for_checkout

Generate a new login token for the customer and update the checkout URL.

```php
public set_login_token_for_checkout(string $checkout_url): string
```

Depending on whether the store is created through the onboarding process
or uses custom API credentials, it generates a login token for the customer.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$checkout_url` | **string** | The original checkout URL. |


**Return Value:**

The updated checkout URL with the login token appended.




***


***
> Automatically generated on 2025-01-03
