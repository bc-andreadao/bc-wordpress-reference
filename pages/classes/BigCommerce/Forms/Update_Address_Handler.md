***

# Update_Address_Handler

Handles the updating and creation of customer addresses.

This class is responsible for validating and processing form submissions for updating or creating
customer addresses. It handles the submission of address forms, validates the data, updates the
customer's address in BigCommerce, and provides appropriate success or error messages.

* Full name: `\BigCommerce\Forms\Update_Address_Handler`
* This class implements:
[`\BigCommerce\Forms\Form_Handler`](./Form_Handler.md)


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

Validates the form submission for address creation or update.

```php
private validate_submission(array $submission, \WP_User $user): \WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** | The form submission data. |
| `$user` | **\WP_User** | The current WordPress user. |


**Return Value:**

A WP_Error object containing any validation errors.




***

### get_address



```php
private get_address(mixed $submitted_address): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submitted_address` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
