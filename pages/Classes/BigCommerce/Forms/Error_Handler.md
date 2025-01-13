***

# Error_Handler

Handles form error management, including storing and retrieving errors for redirection.



* Full name: `\BigCommerce\Forms\Error_Handler`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`PARAM`|public|string|&#039;bc-error&#039;|


## Methods


### form_error

Handle form errors by storing them in a transient and redirecting to the error page.

```php
public form_error(\WP_Error $errors, array $submission, string $redirect = &#039;&#039;): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$errors` | **\WP_Error** | The WP_Error object containing the error details. |
| `$submission` | **array** | The form submission data. |
| `$redirect` | **string** | The URL to redirect to after processing the error. |





***

### get_errors

Retrieve any errors stored in the transient for the current user.

```php
public get_errors(\WP_Error|null $data): \WP_Error|null
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **\WP_Error&#124;null** | Existing error data to potentially override. |


**Return Value:**

The error data, or null if no errors exist.




***


***
> Automatically generated on 2025-01-13
