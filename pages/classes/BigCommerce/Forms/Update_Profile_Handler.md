***

# Update_Profile_Handler

Handles the profile update form submission process.



* Full name: `\BigCommerce\Forms\Update_Profile_Handler`
* This class implements:
[`\BigCommerce\Forms\Form_Handler`](./Form_Handler.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public| |&#039;edit-profile&#039;|


## Methods


### handle_request

Handles the form submission for updating the user profile.

```php
public handle_request(array $submission): void
```








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



```php
private validate_submission(array $submission, \WP_User $user): \WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** |  |
| `$user` | **\WP_User** |  |





***

### get_profile



```php
private get_profile(mixed $submitted_profile): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submitted_profile` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
