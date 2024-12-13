***

# Success_Handler

Handles the success of form submissions by storing a success message, form submission data,
and optionally redirecting the user to a specified URL or reloading the current page.



* Full name: `\BigCommerce\Forms\Success_Handler`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`PARAM`|public|string|&#039;bc-message&#039;|


## Methods


### form_success

Handles the success of a form submission.

```php
public form_success(string $message = &#039;&#039;, array $submission = [], string $redirect = &#039;&#039;, array $data = []): void
```

This method stores the success message, form submission data, and optional extra data as a transient,
and redirects the user to the provided URL (or reloads the current page if no URL is specified).
The transient stores the data temporarily and can be used to display a success message after the redirect.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$message` | **string** | The success message to display to the user after redirect. |
| `$submission` | **array** | The data submitted with the form. |
| `$redirect` | **string** | The URL to redirect to. Leave empty to reload the current URL. |
| `$data` | **array** | Optional data to store with the message (e.g., additional context or metadata). |





***


***
> Automatically generated on 2024-12-13
