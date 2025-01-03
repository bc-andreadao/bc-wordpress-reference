***

# Switch_Currency_Handler

Handles the logic for switching currencies in the BigCommerce cart and triggers success/error actions.

This class interacts with the currency management system and the cart API to update the currency and
recreate the cart if needed, ensuring the correct display and pricing in the switched currency.

* Full name: `\BigCommerce\Forms\Switch_Currency_Handler`
* This class implements:
[`\BigCommerce\Forms\Form_Handler`](./classes/BigCommerce/Forms/Form_Handler.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;switch-currency&#039;|


## Methods


### __construct

Switch_Currency_Handler constructor.

```php
public __construct(\BigCommerce\Currency\Currency $currency, \BigCommerce\Api\v3\Api\CartApi $cart_api): mixed
```

Initializes the handler with the required dependencies: the currency management object and the cart API client.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$currency` | **\BigCommerce\Currency\Currency** | The currency management object. |
| `$cart_api` | **\BigCommerce\Api\v3\Api\CartApi** | The API client for managing carts. |





***

### handle_request

Handles the form submission for switching currency.

```php
public handle_request(array $submission): void
```

Validates the form submission, switches the currency, and recreates the cart if necessary.
If the submission is valid, it triggers the relevant success action or error handling hooks.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** | The submitted form data. |





***


***
> Automatically generated on 2025-01-03
