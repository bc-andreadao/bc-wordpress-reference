***

# Switch_Currency_Handler

Handles the logic for switching currencies in the BigCommerce cart and triggers success/error actions.

This class interacts with the currency management system and the cart API to update the currency and
recreate the cart if needed, ensuring the correct display and pricing in the switched currency.

* Full name: `\BigCommerce\Forms\Switch_Currency_Handler`
* This class implements:
[`\BigCommerce\Forms\Form_Handler`](./Form_Handler.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;switch-currency&#039;|

## Properties


### currency

The currency management object.

```php
private \BigCommerce\Currency\Currency $currency
```






***

### cart_api

The API client for managing carts.

```php
private \BigCommerce\Api\v3\Api\CartApi $cart_api
```






***

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

### should_handle_request



```php
private should_handle_request(mixed $submission): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **mixed** |  |





***

### validate_submission

Validates the form submission data.

```php
private validate_submission(array $submission): \WP_Error
```

Ensures the nonce is valid and the required currency code is provided.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** | The submitted form data. |


**Return Value:**

The validation errors, if any.




***

### maybe_recreate_cart

Recreates the cart if one exists and updates the currency.

```php
private maybe_recreate_cart(string $new_currency_code): void
```

Since it is not possible to update the currency on an already configured cart,
this method deletes the existing cart and recreates it with the new currency code.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$new_currency_code` | **string** | The new currency code to use for the cart. |





***

### format_item_options

Formats the item options for the cart line item.

```php
private format_item_options(array $options, int $product_id): array
```

Converts product options to IDs based on the product's available options.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$options` | **array** | The options to format. |
| `$product_id` | **int** | The product ID. |


**Return Value:**

The formatted options.




***


***
> Automatically generated on 2024-12-10
