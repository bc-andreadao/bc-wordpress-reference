***

# Registration_Handler

Handles user registration requests and form submissions for account creation.



* Full name: `\BigCommerce\Forms\Registration_Handler`
* This class implements:
[`\BigCommerce\Forms\Form_Handler`](./classes/BigCommerce/Forms/Form_Handler.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;register-account&#039;|


## Methods


### __construct

Constructor for the Registration_Handler class.

```php
public __construct(\BigCommerce\Compatibility\Spam_Checker $spam_checker, \BigCommerce\Accounts\Login $login): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$spam_checker` | **\BigCommerce\Compatibility\Spam_Checker** | Instance for checking spam submissions. |
| `$login` | **\BigCommerce\Accounts\Login** | Instance for handling user login. |





***

### handle_request

Handles form submission for user registration.

```php
public handle_request(array $submission): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** | The form submission data. |





***


***
> Automatically generated on 2024-12-31
