***

# Delete_Address_Handler

Handles the deletion of a customer's address from their account.



* Full name: `\BigCommerce\Forms\Delete_Address_Handler`
* This class implements:
[`\BigCommerce\Forms\Form_Handler`](./Form_Handler.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;delete-address&#039;|


## Methods


### handle_request

Handle the address deletion request.

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



```php
private validate_submission(mixed $submission): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
