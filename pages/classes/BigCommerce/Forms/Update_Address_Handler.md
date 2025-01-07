***

# Update_Address_Handler

Handles the updating and creation of customer addresses.

This class is responsible for validating and processing form submissions for updating or creating
customer addresses. It handles the submission of address forms, validates the data, updates the
customer's address in BigCommerce, and provides appropriate success or error messages.

* Full name: `\BigCommerce\Forms\Update_Address_Handler`
* This class implements:
[`\BigCommerce\Forms\Form_Handler`](./classes/BigCommerce/Forms/Form_Handler.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;edit-address&#039;|


## Methods


### handle_request

Handles the form submission for updating or creating an address.

```php
public handle_request(array $submission): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** | The form submission data. |





***


***
> Automatically generated on 2025-01-07
