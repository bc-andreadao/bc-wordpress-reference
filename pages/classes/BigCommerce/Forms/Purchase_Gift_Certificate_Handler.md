***

# Purchase_Gift_Certificate_Handler

Handles the submission and processing of gift certificate purchase forms.



* Full name: `\BigCommerce\Forms\Purchase_Gift_Certificate_Handler`
* This class implements:
[`\BigCommerce\Forms\Form_Handler`](./classes/BigCommerce/Forms/Form_Handler.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;gift-purchase&#039;|


## Methods


### __construct

Purchase_Gift_Certificate_Handler constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CartApi $api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\v3\Api\CartApi** | The Cart API instance. |





***

### handle_request

Handle the gift certificate purchase request.

```php
public handle_request(array $submission): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** | The submitted form data. |





***


***
> Automatically generated on 2025-01-03
