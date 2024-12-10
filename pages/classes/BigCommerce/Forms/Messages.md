***

# Messages

Handles rendering of messages (success or error) above forms or within form submissions.



* Full name: `\BigCommerce\Forms\Messages`




## Methods


### render_messages_above_content

Renders messages above the content.

```php
public render_messages_above_content(string $content): string
```

This method filters whether to show the error/success messages above the content of the form.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$content` | **string** | The original content. |


**Return Value:**

The content with messages prepended.




***

### render_messages

Renders the error or success messages for the form submission.

```php
public render_messages(): string
```

This method checks for stored error or success messages and renders them if available.







**Return Value:**

The rendered error or success messages.




***

### get_error_message



```php
private get_error_message(mixed $key): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$key` | **mixed** |  |





***

### get_success_message



```php
private get_success_message(mixed $key): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$key` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
